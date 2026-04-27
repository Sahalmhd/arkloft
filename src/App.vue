<script setup>
import ServiceUnavailable from './components/ServiceUnavailable.vue'
</script>

<template>
  <div class="h-screen w-screen bg-slate-50 flex items-center justify-center overflow-hidden">
    <div class="max-w-7xl mx-auto w-full h-full flex items-center justify-center p-4 sm:p-6">
      <ServiceUnavailable />
    </div>
  </div>
</template>

<style scoped>
/* Scoped styles are avoided in favor of Tailwind CSS */
</style>
