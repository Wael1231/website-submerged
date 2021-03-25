<template>
  <div class="flex sm:flex-row flex-col sm:space-x-8 space-x-0 sm:space-y-0 space-y-8 items-center justify-center sm:px-8 px-4">
    <img class="xl:h-80 lg:h-72 md:h-64 sm:h-56 h-48" alt="Polus.gg logo" src="../assets/logo.png">
    <div class="text-white">
      <p class="md:text-8xl sm:text-6xl text-4xl font-medium">Polus.gg</p>
      <p class="md:text-2xl sm:text-lg text-sm sm:mt-4 mt-2">The world's best Among Us server</p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Logo",
});
</script>
