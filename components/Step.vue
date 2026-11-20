<script setup lang="ts">
// Paso de <Timeline>. marker: "01", "Nov 2025", etc. Contenido: `### Título` + párrafo.
defineProps<{ marker: string }>()
</script>

<template>
  <div class="ww-step">
    <p class="ww-step-marker">{{ marker }}</p>
    <slot />
  </div>
</template>
