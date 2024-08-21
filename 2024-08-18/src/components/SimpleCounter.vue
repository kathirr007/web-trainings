<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div p-3 rounded bg-gray-2 shadow>
    <button p-1 text-sm rounded-md bg-gray-5 border @click="count++">
      Count is: {{ count }}
    </button>
  </div>
</template>

<style scoped>

</style>
