<template>
  <div class="flex flex-col p-4">
    [Admin Nested Index]
    <p>Go back to default layout and check scrolling works</p>
    <NuxtLink to="/nested" class="text-blue-500">-> [Default - Nested]</NuxtLink>
  </div>
</template>

<script lang="ts" setup>
await useAsyncData('example-admin', () => getPromise());

async function getPromise() {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve('Resolved!');
    }, 250);
  });
}
</script>
