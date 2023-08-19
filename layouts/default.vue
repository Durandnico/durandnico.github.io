<template>
    <v-app>
        <header>
            <!--
            <nav>
                <NuxtLink to="/">Durand Nicolas</NuxtLink>
                <v-card>
    <v-tabs color="deep-purple-accent-4" align-tabs="end">
        <v-tab :value="1" @click="test('/')">Home</v-tab>
       <v-tab :value="3" @click="test('/projects')">projects</v-tab>
       <v-tab :value="2" @click="test('/about')">about</v-tab>
    </v-tabs>
  </v-card>
            </nav>-->
            <Navbar />
            
        </header>

        <div>
            <slot />
        </div>

        <footer>
            <ul>
                <a href="github"></a>
                <a href="linkedin"></a>
            </ul>
        </footer>
    </v-app>
</template>

<script setup lang="ts">


</script>

<style scoped>

</style>