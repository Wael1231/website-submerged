
<template>
  <div class="bg-repeat-x bg-local bg-contain lg:h-96 sm:h-80 h-64 bg-bottom lg:min-h-96 sm:min-h-80 min-h-64 from-transparent via-transparent to-black"
       style="background-image: linear-gradient(to bottom, var(--tw-gradient-stops)), url('https://static.polus.gg/images/cliffs_tile.png')"
  />
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Cliffs",
});
</script>

<style>
.min-h-64 {
  min-height: 16rem;
}

@media (min-width: 640px) {
  .sm\:min-h-80 {
    min-height: 20rem;
  }
}

@media  (min-width: 1024px) {
  .lg\:min-h-96 {
    min-height: 24rem;
  }
}
</style>

