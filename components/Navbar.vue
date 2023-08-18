<template>
    <nav>
        <v-toolbar flat app>
            <span class="title pl-3">DURAND Nicolas</span>
            
            <v-spacer></v-spacer>
            <v-tabs color="#07a70f" class="hidden-sm-and-down">
                <v-tab :value="1" @click="navigateTo('/')" class="pr-6 ml-1 mr-1">Home</v-tab>
                <v-tab :value="3" @click="navigateTo('/projects')" class="pa-6 ml-1 mr-1">projects</v-tab>
                <v-tab :value="2" @click="navigateTo('/about')" class="pa-6 ml-1 mr-1">about</v-tab>
            </v-tabs>
            <v-spacer :class="{hidden: width < 1600 }"></v-spacer>
            
            <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
        </v-toolbar>

    </nav>
</template>

<script setup lang="ts">
import { useDisplay } from 'vuetify'

const { width } = useDisplay()
const drawer = ref(false);


</script>

<style scoped>

.title {
    font-size: 1.25rem;
    font-weight: 400;
    letter-spacing: 0;
    line-height: 1.75rem;
    text-transform: none;
}
</style>