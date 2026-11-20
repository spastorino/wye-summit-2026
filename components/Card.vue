<script setup lang="ts">
// Tarjeta. Contenido en markdown: `### Título` + párrafo o lista.
// icon: ícono de Carbon como clase, por ejemplo "i-carbon-chat"
// eyebrow: etiqueta chica arriba del título
// number: número grande de fondo, abajo a la derecha
// top: borde superior de acento
defineProps<{
  icon?: string
  eyebrow?: string
  number?: string
  top?: boolean
}>()
</script>

<template>
  <div class="ww-card" :class="{ 'ww-card-top': top }">
    <div v-if="icon" class="ww-badge"><div class="ww-icon" :class="icon" /></div>
    <p v-if="eyebrow" class="ww-card-eyebrow">{{ eyebrow }}</p>
    <slot />
    <span v-if="number" class="ww-card-number" aria-hidden="true">{{ number }}</span>
  </div>
</template>
