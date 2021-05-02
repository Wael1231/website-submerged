<template>
  <div class="flex items-center justify-center sm:h-14 h-10 sm:space-x-4 space-x-2 sm:px-8 px-4">
    <span class="inline-flex items-center sm:px-6 sm:py-3 px-4 py-1 border border-transparent shadow-sm text-base font-medium rounded-md text-white bg-[#443062] hover:bg-[#5f3f72] focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-700 cursor-not-allowed">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="-ml-1 mr-3 sm:h-10 h-4 sm:w-10 h-4" fill="currentColor"><path d="M0 3.449L9.75 2.1v9.451H0m10.949-9.602L24 0v11.4H10.949M0 12.6h9.75v9.451L0 20.699M10.949 12.6H24V24l-12.9-1.801"/></svg>
      <div class="flex flex-col items-start">
        <span class="sm:inline hidden text-xs font-light">Coming Soon on</span>
        <span class="sm:hidden text-xs font-light">Soon on</span>
        <span class="sm:text-xl text-xs font-bold">Windows</span>
      </div>
    </span>
    <span class="inline-flex items-center sm:px-6 sm:py-3 px-4 py-1 border border-transparent shadow-sm text-base font-medium rounded-md text-white bg-[#443062] hover:bg-[#5f3f72] focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-700 cursor-not-allowed">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" class="-ml-1 mr-3 sm:h-10 h-4 sm:w-10 h-4" fill="currentColor"><path d="M22.018 13.298l-3.919 2.218-3.515-3.493 3.543-3.521 3.891 2.202a1.49 1.49 0 0 1 0 2.594zM1.337.924a1.486 1.486 0 0 0-.112.568v21.017c0 .217.045.419.124.6l11.155-11.087L1.337.924zm12.207 10.065l3.258-3.238L3.45.195a1.466 1.466 0 0 0-.946-.179l11.04 10.973zm0 2.067l-11 10.933c.298.036.612-.016.906-.183l13.324-7.54-3.23-3.21z"/></svg>
      <div class="flex flex-col items-start">
        <span class="sm:inline hidden text-xs font-light">Coming Soon on</span>
        <span class="sm:hidden text-xs font-light">Soon on</span>
        <span class="sm:text-xl text-xs font-bold">Google Play</span>
      </div>
    </span>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Downloads",
});
</script>
