<template>
  <div class="h-full pt-4">
    [Default Layout]

    <slot />
  </div>
</template>

<script setup lang="ts">
useHead({
  bodyAttrs: { class: 'h-full bg-gray-900 text-white' },
  htmlAttrs: { class: 'h-full' },
})
</script>
