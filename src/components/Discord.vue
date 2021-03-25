<template>
  <div class="flex items-center justify-center sm:px-8 px-4 pb-6">
    <p class="text-white font-medium md:text-2xl sm:text-lg text-sm mr-2 -mt-1">Stay up to date on our</p>
    <a href="https://discord.gg/polus" target="_blank" class="block">
      <img class="object-contain sm:h-14 h-8" alt="Discord logo" src="../assets/discord.png">
    </a>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Discord",
});
</script>
