<template>
    <v-card
      class="mx-auto card"
      color="#494d64"
      id="card"
    >
    <v-card-title class="title">
      {{title}}
    </v-card-title>


        <v-img
        :src="img"
        height="150px"
        width="250px"
        :cover="cover"
        ></v-img>
  
      

        <v-card-text>
            {{ desc }}
        </v-card-text>

        <v-divider class="mx-4"></v-divider>
        <v-card-text>
            <v-chip v-for="chip in chips" :key="chip.valueOf()" class="chip">{{ chip }}</v-chip>
        </v-card-text>
    </v-card>
  </template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    data: () => ({
        show:false
    }),
    props: {
        title : {
            type: String,
            default: "This is the title"
        },
        desc: {
            type: String,
            default: "this is the description part"
        },
        img: {
            type: String,
            default: "img"
        },
        chips: {
            type: Array<String>,
            default: []
        },
        cover :{
            type: Boolean,
            default: true
        }

    }
})
</script>

<style scoped>

* {
    color: #c6d0f5
}

.card {
    max-width: 250px;
}

.title {
    position: relative;
    z-index: 10;
    width: 100%;
    text-align: center;
}

.chip {
    margin: 1.5px;
    font-size:x-small !important;
}

#card {
    transition: all 0.27s ease-in-out;
}
#card:hover{
    transform: translateY(-8%) !important;
}
</style>