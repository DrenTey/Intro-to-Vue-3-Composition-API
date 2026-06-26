<script setup>
import { ref } from 'vue'
import ProductDisplay from '@/components/ProductDisplay.vue';
import ProductDetails from './components/ProductDetails.vue';
const cart = ref(0)
const premium = ref(false)
const details = ref([])
</script>
  
<template>
  <div class="nav-bar"></div>
  <div class="cart">Cart({{ cart }})</div>
  <ProductDisplay :premium="premium"></ProductDisplay>
  <ProductDetails :details="details"></ProductDetails>
  </template>