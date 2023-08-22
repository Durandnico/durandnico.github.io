<template>
    <v-card
      class="mx-auto card"
      color="#494d64"
    >
    <v-card-title class="title">
      {{title}}
    </v-card-title>

      <v-img
        :src="img"
        height="200px"
        width="250px"
        cover
      ></v-img>
  
      

        <v-card-text>
            {{ desc }}
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
            type: String
        },
        desc: {
            type: String
        },
        img: {
            type: String,
            default: "img"
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
    position: absolute;
    z-index: 10;
    left: 30px;
}
</style>