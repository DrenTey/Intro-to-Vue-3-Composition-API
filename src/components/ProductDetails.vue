<script setup>
import { ref, computed } from 'vue'


const props2 = defineProps({
    details: {
        type: Array,
        required: true
    }
})
</script>

<template>
        <ul>
          <li v-for="detail in props2.details">{{ detail }}</li>
        </ul>
</template>