<template>
    <h1>Projects</h1>
    <div class="main">
        <h2>2023</h2>
        <Projet class="item" img="images/durandnico.png" title="Ce site" desc="Ce site me sert de 'vitrine' personnalisée. Une presentation sommaire de mes compétences en développement et de mon investissement" :chips="['Website', 'NuxtJs', 'Personnel']"/>
        <Projet class="item" img="images/accueil.png" title="AP8" desc="L'AP8 est une application tablette re-configurable de gestion, controle et test des systèmes d'alarmes VIGInet" :chips="['Applicatif', 'ElectronJs', 'VueJs', 'NodeJS', 'SCRUM', 'Professionnel']"/>
        <Projet class="item" :cover="false" img="images/iapau_round.png" title="IA Pau" desc="Réalisation d'une application pour IA Pau permettant la création et l'administration de data challenges." :chips="['Website', 'MySQL', 'Team', 'Universitaire']"/>
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Irréductible palois"  :chips="['Website', 'MySQL', 'Universitaire']"/>
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Démineur"  :chips="['Game', 'C', 'X11', 'Universitaire']"/>

        <h2>2022</h2>
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="OwOption" desc="Un site web permettant la gestion de compte, répartition d'élèves dans leurs options via un algorithme de mariage stabe" :chips="['Website', 'Team', 'Universitaire']"/>
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Huffman" desc="Programme de compression du codage de Huffman en binaire avec gestion des arguments d'entrés" :chips="['C', 'Compression', 'Binaire', 'Team', 'Universitaire']" />
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Analyse de données"  :chips="['Bash', 'Team', 'Universitaire']" />

        <h2>2021</h2>
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4" desc="Un jeu de puissance 4 avec la possibilité de jouer contre une IA utilisant l'algorithme minimax" :chips="['Game', 'C', 'IA', 'Universitaire']" />

    </div>
</template>

<script setup>

</script>

<style scoped>

h1 {
    width: 65%;
    margin: 0 auto;
    margin-top: 1rem;
    text-align:left;
}

h2 {
    position: relative;
    left: 5%;
    width: 100%;
    margin-top: 3rem;
}
.main {
    position: relative;
    max-width: 75%;
    margin: 0 auto;
    padding: 0;
    margin-bottom: 0;
    gap:1.5rem;
}


.main {
  display: -webkit-box;     /* iOS 6-, Safari 3.1-6 */
  display: -moz-box;        /* Firefox 19- */
  display: -ms-flexbox;     /* IE 10 */
  display: -webkit-flex;    /* Chrome */
  display: flex;            /* Opera 12.1, Firefox 20+ */
  align-items: flex-start;

  /* iOS 6-, Safari 3.1-6 */
  -webkit-box-orient: horizontal;
  -webkit-lines: multiple;  /* Only here for informative purpose, this line is what should have made it work, it has never been implemented */ 

  /* Firefox 19- */
  -moz-flex-flow: row wrap;
  -moz-box-lines: multiple; /* Only here for informative purpose, this line is what should have made it work, it has never been implemented */ 

  /* Chrome */
  -webkit-flex-flow: row wrap;

  /* IE10 */
  -ms-flex-flow: row wrap;

  /* Opera 12.1, Firefox 20+ */
  flex-flow: row wrap;
}
.item {
    height: max-content;
  margin: 10px !important;
  -webkit-box-flex: flex-start;    /* iOS 6-, Safari 3.1-6 */
  -moz-box-flex: 1.0;        /* Firefox 19- */
  -webkit-flex: flex-start;        /* Chrome */
  -ms-flex: flex-start;            /* IE10 */
  flex: flex-start;                /* Opera 12.1, Firefox 20+ */
  align-self: left;
}
</style>