<script setup lang="ts">
// Un lado de <Compare>. El contenido es una lista markdown (`- ...`).
defineProps<{
  year: string
  headline: string
  dark?: boolean
}>()
</script>

<template>
  <div class="ww-side" :class="{ 'ww-side-dark': dark }">
    <p class="ww-side-year">{{ year }}</p>
    <p class="ww-side-headline">{{ headline }}</p>
    <slot />
  </div>
</template>
