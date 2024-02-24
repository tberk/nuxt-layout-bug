<template>
  <div class="p-4 flex flex-col gap-2">
    [Nested Index] - This page should be scrollable

    <p>
      - Check scrolling works if you came from the landing page
    </p>
    <NuxtLink to="/admin/nested" class="text-blue-500"> -> /admin/nested</NuxtLink>

    <div class="w-full h-[4000px] border">
      [Scrollable content]
      <p>
        Classes from admin layout leaks to default layout
        <br />
        Check body class while navigating
      </p>
    </div>
  </div>
</template>

<script lang="ts" setup>
await useAsyncData('example', () => getPromise());

async function getPromise() {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve('Resolved!');
    }, 250);
  });
}
</script>
