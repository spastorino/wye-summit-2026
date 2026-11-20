<script setup lang="ts">
// Fila de etapa con estado. El contenido (markdown) es la descripción.
// status: "completa" (pastilla llena) | "casi" (pastilla punteada)
defineProps<{
  eyebrow?: string
  title: string
  status?: 'completa' | 'casi'
}>()
</script>

<template>
  <div class="ww-stage">
    <div class="ww-stage-head">
      <p v-if="eyebrow" class="ww-card-eyebrow">{{ eyebrow }}</p>
      <h3>{{ title }}</h3>
    </div>
    <div class="ww-stage-body"><slot /></div>
    <p v-if="status" class="ww-pill" :class="`ww-pill-${status}`">
      <span v-if="status === 'completa'" class="i-carbon-checkmark ww-pill-icon" />
      {{ status === 'completa' ? 'Completa' : 'Casi' }}
    </p>
  </div>
</template>
