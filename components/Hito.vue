<script setup lang="ts">
// Un hito de <Hitos>: fecha, nombre y una línea de descripción (el contenido)
defineProps<{ date: string; name: string }>()
</script>

<template>
  <div class="ww-hito">
    <p class="ww-hito-date">{{ date }}</p>
    <p class="ww-hito-name">{{ name }}</p>
    <p class="ww-hito-desc"><slot /></p>
  </div>
</template>
