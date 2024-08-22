<script setup lang="ts">
import { ref } from 'vue'

const isDevBuild = ref(import.meta.env.MODE === 'development')
</script>

<template>
  <h2 mb-4>
    Trainings - Kathirr007
  </h2>

  <ul>
    <li><a href="/2024/vue-js-training/">Vue.js Training</a></li>
  </ul>
</template>

<style scoped>

</style>
