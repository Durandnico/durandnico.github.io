<template>
   <h1>Projects</h1>
    <div class="main">
        <h2>2024</h2>
        <Projet class="item" :cover="false" img="images/NN.png" title="Neural network C++" desc="Developpement de ma propre librairy de réseau neuronal artificiel et autre algorithmes de prédictions en C++" :chips="['IA', 'C++', 'Neural Network', 'Personnel']"/>

        <h2>2023</h2>
        <Projet class="item" img="images/prezzup.png" title="Data battle IA Pau" desc="Analyse audiovisuelle d'un pitch vidéo via intelligence artificielle pour l'entreprise Prezzup" :chips="['IA', 'PyTorch', 'Analyse audiovisuelle', 'whisper', 'mediapipe', 'Personnel']"/>
        <Projet class="item" :cover="false" img="images/Spotiflop.png" title="Spotiflop" desc="Site web de streaming audio personnel" :chips="['Website', 'JEE', 'Springboot', 'VueJs', 'PostgresSQL', 'Team', 'Universitaire']"/>
        <Projet class="item" img="images/durandnico.png" title="Ce site" desc="Ce site me sert de 'vitrine' personnalisée. Une presentation sommaire de mes compétences en développement et de mon investissement" :chips="['Website', 'NuxtJs', 'Personnel']"/>
        <Projet class="item" img="images/accueil.png" title="AP8" desc="L'AP8 est une application tablette re-configurable de gestion, controle et test des systèmes d'alarmes VIGInet" :chips="['Applicatif', 'ElectronJs', 'VueJs', 'NodeJS', 'SCRUM', 'Professionnel']"/>
        <Projet class="item" :cover="false" img="images/iapau_round.png" title="IA Pau" desc="Réalisation d'une application pour IA Pau permettant la création et l'administration de data challenges." :chips="['Website', 'MySQL', 'Team', 'Universitaire']"/>
        <Projet class="item" img="images/IR_website.png" title="Irréductible palois" desc="File rouge de mon 2ème semetre en 1ère année, Site web sur ma famille de CY Tech avec une page de vente et gestion des utilisateurs" :chips="['Website', 'MySQL', 'Universitaire']"/>
        <Projet class="item" img="images/minesweeper.png" title="Démineur"  :chips="['Game', 'C', 'X11', 'Universitaire']"/>

        <h2>2022</h2>
        <Projet class="item" img="images/owo.png" title="OwOption" desc="Un site web permettant la gestion de compte, répartition d'élèves dans leurs options via un algorithme de mariage stabe" :chips="['Website', 'Team', 'Universitaire']"/>
        <Projet class="item" img="images/huffman.png" title="Huffman" desc="Programme de compression du codage de Huffman en binaire avec gestion des arguments d'entrés" :chips="['C', 'Compression', 'Binaire', 'Team', 'Universitaire']" />

        <h2>2021</h2>
        <Projet class="item" img="images/p4.png" title="Puissance 4" desc="Un jeu de puissance 4 avec la possibilité de jouer contre une IA utilisant l'algorithme minimax" :chips="['Game', 'C', 'IA', 'Universitaire']" />

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