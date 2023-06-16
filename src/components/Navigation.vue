<template>
  <nav class="nav">
    <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
      <div class="relative flex items-center justify-between h-16">
        <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
          <button @click="menuOpen = !menuOpen"
                  type="button"
                  class="inline-flex items-center justify-center p-2 rounded-full text-blue-400 hover:text-white hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
                  aria-controls="mobile-menu"
                  aria-expanded="false">
            <span class="sr-only">
              Open main menu
            </span>
            <svg xmlns="http://www.w3.org/2000/svg"
                 viewBox="0 0 24 24"
                 class="block h-6 w-6"
                 fill="none"
                 stroke="currentColor"
                 aria-hidden="true">
              <path stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    :d="menuOpen ? 'M6 18L18 6M6 6l12 12' : 'M4 6h16M4 12h16M4 18h16'" />
            </svg>
          </button>
        </div>
        <div class="flex-1 flex items-center justify-center sm:items-stretch sm:justify-start">
          <div class="flex-shrink-0 flex items-center">
            <Logo class="block h-8 w-auto"
                  width="64"
                  height="64" />
            <p class="block ml-2 text-white font-black">
              Submerged
            </p>
          </div>
          <div class="hidden sm:block sm:ml-6">
            <div class="flex space-x-4">
              <a href="/"
                 class="bg-[#44b0df] text-white px-3 py-2 rounded-full text-sm font-medium">
                Home
              </a>
              <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white px-3 py-2 rounded-full text-sm font-medium">
                Leaderboards
              </span>
              <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white px-3 py-2 rounded-full text-sm font-medium">
                Contact us
              </span>
              <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white px-3 py-2 rounded-full text-sm font-medium">
                Staff
              </span>
              <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white px-3 py-2 rounded-full text-sm font-medium">
                Credits
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div v-if="menuOpen"
         class="sm:hidden"
         id="mobile-menu">
      <div class="px-2 pt-2 pb-3 space-y-1">
        <a href="/"
           class="bg-[#5f3f72] text-white block px-3 py-2 rounded-full text-base font-medium">
          Home
        </a>
        <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white block px-3 py-2 rounded-full text-base font-medium">
          Leaderboards
        </span>
        <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white block px-3 py-2 rounded-full text-base font-medium">
          Contact
        </span>
        <span class="cursor-not-allowed text-blue-300 hover:bg-blue-700 hover:text-white block px-3 py-2 rounded-full text-base font-medium">
          Staff
        </span>
        <span class="text-blue-300 hover:bg-blue-700 hover:text-white px-3 py-2 rounded-full text-sm font-medium">
           Credits
       </span>
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Logo from "./Logo.vue";

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Navigation",
  components: {
    Logo,
  },
  data() {
    return {
      menuOpen: false,
    };
  },
});
</script>

<style scoped>
.nav {
  background: rgba(0, 0, 0, 0.33);
}
</style>
