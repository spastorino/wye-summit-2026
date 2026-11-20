<script setup lang="ts">
// Cita grande. El primer párrafo es la cita; los siguientes, comentario.
// size: xl (por defecto) | lg   ·   bar: línea de acento a la izquierda
defineProps<{
  author?: string
  size?: 'xl' | 'lg'
  bar?: boolean
}>()
</script>

<template>
  <div class="ww-quote" :class="[`ww-quote-${size ?? 'xl'}`, { 'ww-quote-bar': bar }]">
    <slot />
    <div v-if="author" class="ww-quote-author">{{ author }}</div>
  </div>
</template>
