<template>
  <div class="flex items-center justify-center sm:h-14 h-10 sm:space-x-4 space-x-2 sm:px-8 px-4">
    <img class="cursor-not-allowed object-scale-down h-full" alt="Android download button" src="../assets/android.png">
    <img class="cursor-not-allowed object-scale-down h-full" alt="Windows download button" src="../assets/windows.png">
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Downloads",
});
</script>
