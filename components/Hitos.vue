<script setup lang="ts">
// Bloque oscuro con una línea de tiempo corta de <Hito>
defineProps<{ title?: string }>()
</script>

<template>
  <div class="ww-hitos">
    <p v-if="title" class="ww-hitos-title">{{ title }}</p>
    <div class="ww-hitos-list"><slot /></div>
  </div>
</template>
