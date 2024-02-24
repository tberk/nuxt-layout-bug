<template>
  <div class="h-full pt-4">
    [Admin Layout]

    <slot />
  </div>
</template>

<script setup lang="ts">
useHead({
  htmlAttrs: { class: 'h-full bg-gray-900 text-white' },
  bodyAttrs: { class: 'h-full overflow-hidden this-class-should-not-be-on-default-layout' },
})
</script>
