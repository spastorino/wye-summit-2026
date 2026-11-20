<script setup lang="ts">
// Tarjeta de proyecto dentro de <Projects>: nombre grande y, opcional,
// una línea de descripción (el contenido).
defineProps<{ name: string }>()
</script>

<template>
  <div class="ww-project">
    <p class="ww-project-name">{{ name }}</p>
    <p v-if="$slots.default" class="ww-project-desc"><slot /></p>
  </div>
</template>
