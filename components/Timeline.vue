<script setup lang="ts">
// Línea de tiempo de pasos (<Step>). compact: marcadores más chicos (para fechas)
defineProps<{ compact?: boolean }>()
</script>

<template>
  <div class="ww-timeline" :class="{ 'ww-timeline-compact': compact }"><slot /></div>
</template>
