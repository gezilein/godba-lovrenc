<script setup lang="ts">
import consola from "consola";

import { useDataStore } from "@/store/data";

const dataStore = useDataStore();

onMounted(async () => {
  await dataStore.$load({ name: "app-data" }).catch((error: any) => consola.log(error));
});

useHead({
  title: "Pihalna godba PGD Lovrenc na Pohorju",
  meta: [
    {
      name: "description",
      content: "Predstavitev godba PGD Lovrenc na Pohorju",
    },
  ],
});
</script>

<template>
  <div id="bar" />
  <router-view />
</template>

<style lang="scss">
@import "App.scss";
</style>
