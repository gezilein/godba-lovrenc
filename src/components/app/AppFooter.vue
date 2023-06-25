<script setup lang="ts">
// const version = ref(import.meta.env.VITE_APP_VERSION)
const year = new Date().getFullYear();
</script>

<template>
  <div class="mt-4 layout-footer">
    <span class="font-medium ml-2">Godba na pihala PGD Lovrenc na Pohorju - &copy;{{ year }}</span>
  </div>
</template>

<style scoped></style>
