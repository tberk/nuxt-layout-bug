<template>
  <div>
    <ChadToggle v-model:pressed="toggle">Toggle</ChadToggle>
    {{ toggle }}
  </div>
</template>

<script lang="ts" setup>
const toggle = ref(false)
</script>
