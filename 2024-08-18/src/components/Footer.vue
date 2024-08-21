<script setup lang="ts">
import dayjs from 'dayjs'
import { useSlideContext } from '@slidev/client'

const { $slidev } = useSlideContext()
</script>

<template>
  <div abs-b m-2 flex justify-between text-gray op35 class="footer-contents">
    <div flex flex-1>
      Vue.js Training | Kathiravan K | {{ dayjs().format('DD/MM/YYYY') }}
    </div>
    <div>
      Company Confidential @ Capgemini {{ dayjs().format('YYYY') }}. All rights reserved. | {{ $slidev.nav.currentPage }}
    </div>
  </div>
</template>

<style scoped>
.footer-contents {
  font-size: 8px;
}
</style>
