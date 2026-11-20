<script setup lang="ts">
// Etiqueta de grupo al principio de cada fila de <Projects> (por ejemplo "AWS")
defineProps<{ title: string }>()
</script>

<template>
  <div class="ww-project-label">
    <p class="ww-project-label-title">{{ title }}</p>
  </div>
</template>
