<template>
  <div class="h-full pt-4">
    [Default Layout]

    <slot />
  </div>
</template>

<script setup lang="ts">
useHead({
  htmlAttrs: { class: 'h-full default-layout-html-class' },
  bodyAttrs: { class: 'h-full default-layout-body-class bg-gray-900 text-white' },
})
</script>
