<template>
    <h2>Projects</h2>
    <div class="main">
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4 en C" desc="Le tzatzíki est un mezzé grec et turc qui peut être utilisé comme sauce ou comme entrée. Le mot serait dérivé du turc cacık qui désigne une sorte de condiment." />
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4 en C" desc="Le tzatzíki est un mezzé grec et turc qui peut être utilisé comme sauce ou comme entrée. Le mot serait dérivé du turc cacık qui désigne une sorte de condiment." />
        <Projet class="item" img="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" title="Puissance 4 en C" desc="Le tzatzíki est un mezzé grec et turc qui peut être utilisé comme sauce ou comme entrée. Le mot serait dérivé du turc cacık qui désigne une sorte de condiment." />
    </div>
</template>

<script setup>

</script>

<style scoped>

h2 {
    width: 65%;
    margin: 0 auto;
    margin-top: 1rem;
    text-align:left;
}

.main {
    position: relative;
    max-width: 75%;
    margin: 0 auto;
    margin-top: 2rem;
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