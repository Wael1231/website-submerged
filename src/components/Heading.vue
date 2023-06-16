<template>
  <div class="flex sm:flex-row flex-col sm:space-x-8 space-x-0 sm:space-y-0 space-y-8 items-center justify-center sm:px-8 px-4">
    <Logo class="xl:w-80 xl:h-80 lg:w-72 lg:h-72 md:w-64 md:h-64 sm:w-56 sm:h-56 w-48 h-48"
          width="676"
          height="676" />
    <div class="text-white">
      <p class="md:text-8xl sm:text-6xl text-4xl font-medium">
        Submerged
      </p>
      <p class="md:text-2xl sm:text-lg text-sm sm:mt-4 mt-2">
        An Among Us mod which adds a new underwater map
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Logo from "./Logo.vue";

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Heading",
  components: {
    Logo,
  },
});
</script>
