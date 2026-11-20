<script setup lang="ts">
// Slide de contenido: eyebrow + título (el `# ...` del markdown) + cuerpo.
// Frontmatter: eyebrow, tight (menos espacio bajo el título)
defineProps<{
  eyebrow?: string
  tight?: boolean
}>()
</script>

<template>
  <div class="slidev-layout ww ww-contenido" :class="{ 'ww-tight': tight }">
    <p v-if="eyebrow" class="ww-eyebrow">{{ eyebrow }}</p>
    <slot />
  </div>
</template>
