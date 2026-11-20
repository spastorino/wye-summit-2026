<script setup lang="ts">
// Slide de declaración sobre fondo oscuro: portada y cierre.
// Frontmatter: eyebrow, align (center | end), size (xl | lg),
//              logo (top | bottom): logo de Rust en el color de acento,
//              bar: barrita de acento arriba
defineProps<{
  eyebrow?: string
  align?: 'center' | 'end'
  size?: 'xl' | 'lg'
  logo?: 'top' | 'bottom'
  bar?: boolean
}>()
</script>

<template>
  <div
    class="slidev-layout ww ww-dark ww-declaracion"
    :class="[`ww-align-${align ?? 'center'}`, `ww-size-${size ?? 'xl'}`]"
  >
    <div v-if="logo" class="ww-logo" :class="`ww-logo-${logo}`" role="img" aria-label="Logo de Rust" />
    <div v-if="bar" class="ww-bar" />
    <p v-if="eyebrow" class="ww-eyebrow">{{ eyebrow }}</p>
    <slot />
  </div>
</template>
