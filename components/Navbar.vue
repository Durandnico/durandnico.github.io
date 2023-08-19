<template>
    <nav>
        <v-toolbar flat app dark color="#222222">
            <span class="title pl-10 font-weight-bold c-white">DURAND Nicolas</span>
            
            <v-spacer></v-spacer>
            <v-tabs color="#07a70f" dark class="hidden-sm-and-down -ml-64">
                <v-tab :value="1" @click="navigateTo('/')" class="pr-6 ml-1 mr-1">Home</v-tab>
                <v-tab :value="3" @click="navigateTo('/projects')" class="pa-6 ml-1 mr-1 c-white">projects</v-tab>
                <v-tab :value="2" @click="navigateTo('/about')" class="pa-6 ml-1 mr-16 c-white">about</v-tab>
            </v-tabs>
            <v-spacer :class="{hidden: width < 1600 }"></v-spacer>
            
            <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
        </v-toolbar>

        <v-navigation-drawer app v-model="drawer" class="hidden-md-and-up">
            <v-list-item class=ma-3>
                <v-list-item-content>
                    <v-list-item-title class="title font-weight-bold">
                        Durand Nicolas {{test}}
                    </v-list-item-title>
                </v-list-item-content>
            </v-list-item>

            <v-divider></v-divider>
            
                <v-list nav>
                        <v-list-item @click="{drawer = false; navigateTo('/'); test=1}" class="hv">
                            <span class="ml-6 font-500">home</span>
                        </v-list-item>

                        <v-list-item @click="{drawer = false; navigateTo('/projects'); test=3}" class="hv">
                            <span :value="3" class="pa-4 ml-2 pr-32">projects</span>
                        </v-list-item>
                       
                        <v-list-item  @click="{drawer = false; navigateTo('/projects'); test=2}" class="hv">
                            <span :value="2" class="pa-4 ml-2 pr-32">about</span>
                        </v-list-item>

                </v-list>
        </v-navigation-drawer>
    </nav>
</template>

<script setup lang="ts">
import { useDisplay } from 'vuetify'

const { width } = useDisplay()
const drawer = ref(false);
const test = ref(null)


</script>

<style scoped>

.title {
    font-size: 1.25rem;
    font-weight: 400;
    letter-spacing: 0;
    line-height: 1.75rem;
    text-transform: none;
}

.router-link-exact-active {
    color:#12b488;
}

:not(.router-link-exact-active) {
    color: white
}

.hv:hover{
    background-color: rgba(0,0,0,0.05);
}

</style>