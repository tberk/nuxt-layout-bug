<template>
  <div class="h-full pt-4 bg-gray-900 text-white">
    [Admin Layout]

    <slot />
  </div>
</template>

<script setup lang="ts">
useHead({
  htmlAttrs: { class: 'h-full admin-layout-html-class' },
  bodyAttrs: { class: 'h-full overflow-hidden admin-layout-body-class bg-gray-900 text-white' },
})
</script>
