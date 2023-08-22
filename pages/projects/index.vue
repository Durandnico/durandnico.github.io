<template>
    <div class="main">
        <Projet img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4 en C" desc="Un distributeur automatique pour des poissons rouges. Imprimable en 3D, il fonctionne avec un servo-moteur, relié à une Raspberry-Pi." />
        <Projet img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4 en C" desc="Un distributeur automatique pour des poissons rouges. Imprimable en 3D, il fonctionne avec un servo-moteur, relié à une Raspberry-Pi." />
    </div>
</template>

<script setup>

</script>

<style scoped>

.main {
    position: relative;
    width: 90%;
    margin: 0 auto;
    margin-top: 2rem;
    display: grid;
    gap: 1.5rem;
}

.main * {

    height: max-content;
}
</style>