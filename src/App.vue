<script setup>
import { ref } from 'vue'
import socksGreenImage from './assets/images/socks_green.jpeg'
import socksBlueImage from './assets/images/socks_blue.jpeg'
const product = ref('Socks')
const image = ref(socksBlueImage)
const url1 = ref('https://google.com')
const url2t = ref("Link2")
const url = ref(url1)
// Add a url ref
//Bind the url to an anchor tag’s href attribute
</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <img v-bind:src="image">
        <a :href="url"> {{ url2t }}</a>
      </div>
      <div class="product-info">
        <h1>{{ product }}</h1>
      </div>
    </div>
  </div>
</template>