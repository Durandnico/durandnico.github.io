<template>
    <nav class="header-nav">
        <v-toolbar flat app dark color="rgb(36, 39, 58, 0.7)">
            <div class="test">

                <span class="title pl-10 font-weight-bold pa-4" @click="{navMenu = 1; navigateTo('/')}">> durandnico.github.io</span>
                
            <v-tabs color="#a6e3a1" dark class="hidden-sm-and-down -ml-24" v-model="navMenu" >
                <v-tab :value="1" @click="navigateTo('/')" class="pr-6 ml-1 mr-1">HOME</v-tab>
                <v-tab :value="2" @click="navigateTo('/cv')" class="pa-6 ml-1 mr-1">CV</v-tab>
                <v-tab :value="3" @click="navigateTo('/projects')" class="pa-6 ml-1 mr-1 case-upper ">projects</v-tab>
                <v-tab :value="4" @click="navigateTo('/about')" class="pa-6 ml-1 mr-16">README.md</v-tab>
            </v-tabs>
            
            <SocialMedia class="pa-4 pr-12 hidden-md-and-down" />

            <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
        </div>
        </v-toolbar>

        <v-navigation-drawer app dark color="#303446" v-model="drawer" class="hidden-md-and-up">
            <v-list-item class=ma-3>
                    <v-list-item-title class="title font-weight-bold">
                        Durand Nicolas
                    </v-list-item-title>
                </v-list-item>
                
                <v-divider></v-divider>
            
                <v-list nav>
                        <v-list-item @click="{drawer = false; navigateTo('/');}" class="hv">
                            <span class="pa-4 ml-2 pr-32">HOME</span>
                        </v-list-item>

                        <v-list-item @click="{drawer = false; navigateTo('/cv');}" class="hv">
                            <span class="pa-4 ml-2 pr-32">CV</span>
                        </v-list-item>

                        <v-list-item @click="{drawer = false; navigateTo('/projects');}" class="hv">
                            <span class="pa-4 ml-2 pr-32">PROJECTS</span>
                        </v-list-item>

                        <v-list-item  @click="{drawer = false; navigateTo('/about');}" class="hv">
                            <span class="pa-4 ml-2 pr-32">README.md</span>
                        </v-list-item>

                </v-list>
        </v-navigation-drawer>
    </nav>
</template>

<script lang="ts">
export default {
    data: () => ({
        drawer: false,
        navMenu: null
    })
}
</script>

<style scoped>

.v-tab {
    text-transform: none;
}

.test {
    display:flex;
    flex-direction: row;
    justify-content: space-between;
    width:100%;
}
.header-nav {
    z-index: 99;
}

.header-nav * {
    z-index: 99;
}
.title {
    font-size: 1.25rem;
    font-weight: 400;
    letter-spacing: 0;
    line-height: 1.75rem;
    text-transform: none;
}

.router-link-exact-active {
    color:#a6d189;
}

:not(.router-link-exact-active) {
    color: #c6d0f5
}

.hv:hover{
    background-color: rgba(0,0,0,0.05);
}

</style>