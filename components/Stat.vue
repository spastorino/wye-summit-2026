<script setup lang="ts">
// Número grande con su etiqueta (el contenido del componente)
defineProps<{ value: string }>()
</script>

<template>
  <div class="ww-stat">
    <p class="ww-stat-value">{{ value }}</p>
    <p class="ww-stat-label"><slot /></p>
  </div>
</template>
