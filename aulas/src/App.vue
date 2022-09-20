<script setup>
import { RouterLink, RouterView } from "vue-router";
import TheHeader from "./components/TheHeader.vue";
import AsDiretivas from "./components/AsDiretivas.vue";
import OsLoops from "./components/OsLoops.vue";
</script>

<template>
  <TheHeader />
  <AsDiretivas />
  <OsLoops />

  <RouterView />
</template>

