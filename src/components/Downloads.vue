<template>
  <div class="flex items-center justify-center sm:h-14 h-10 sm:space-x-4 space-x-2 sm:px-8 px-4">
    <a href="https://store.steampowered.com/app/1653240/Polusgg/"
       target="_blank"
       rel="noopener"
       class="inline-flex items-center sm:px-6 sm:py-3 px-4 py-1 border border-transparent shadow-sm text-base font-medium rounded-md text-white bg-[#443062] hover:bg-[#5f3f72] focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-700">
      <svg xmlns="http://www.w3.org/2000/svg"
           viewBox="0 0 24 24"
           class="-ml-1 mr-3 sm:h-10 h-4 sm:w-10 h-4"
           fill="currentColor">
        <path d="M11.979 0C5.678 0 .511 4.86.022 11.037l6.432 2.658c.545-.371 1.203-.59 1.912-.59.063 0 .125.004.188.006l2.861-4.142V8.91c0-2.495 2.028-4.524 4.524-4.524 2.494 0 4.524 2.031 4.524 4.527s-2.03 4.525-4.524 4.525h-.105l-4.076 2.911c0 .052.004.105.004.159 0 1.875-1.515 3.396-3.39 3.396-1.635 0-3.016-1.173-3.331-2.727L.436 15.27C1.862 20.307 6.486 24 11.979 24c6.627 0 11.999-5.373 11.999-12S18.605 0 11.979 0zM7.54 18.21l-1.473-.61c.262.543.714.999 1.314 1.25 1.297.539 2.793-.076 3.332-1.375.263-.63.264-1.319.005-1.949s-.75-1.121-1.377-1.383c-.624-.26-1.29-.249-1.878-.03l1.523.63c.956.4 1.409 1.5 1.009 2.455-.397.957-1.497 1.41-2.454 1.012H7.54zm11.415-9.303c0-1.662-1.353-3.015-3.015-3.015-1.665 0-3.015 1.353-3.015 3.015 0 1.665 1.35 3.015 3.015 3.015 1.663 0 3.015-1.35 3.015-3.015zm-5.273-.005c0-1.252 1.013-2.266 2.265-2.266 1.249 0 2.266 1.014 2.266 2.266 0 1.251-1.017 2.265-2.266 2.265-1.253 0-2.265-1.014-2.265-2.265z"/>
      </svg>
      <div class="flex flex-col items-start">
        <span class="sm:inline hidden text-xs font-light">
          Available on
        </span>
        <span class="sm:hidden text-xs font-light">
          Play on
        </span>
        <span class="sm:text-xl text-xs font-bold">
          Steam
        </span>
      </div>
    </a>
    <span class="inline-flex items-center sm:px-6 sm:py-3 px-4 py-1 border border-transparent shadow-sm text-base font-medium rounded-md text-white bg-[#443062] hover:bg-[#5f3f72] focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-700 cursor-not-allowed">
      <svg xmlns="http://www.w3.org/2000/svg"
           viewBox="0 0 24 24"
           class="-ml-1 mr-3 sm:h-10 h-4 sm:w-10 h-4"
           fill="currentColor">
        <path d="M22.018 13.298l-3.919 2.218-3.515-3.493 3.543-3.521 3.891 2.202a1.49 1.49 0 0 1 0 2.594zM1.337.924a1.486 1.486 0 0 0-.112.568v21.017c0 .217.045.419.124.6l11.155-11.087L1.337.924zm12.207 10.065l3.258-3.238L3.45.195a1.466 1.466 0 0 0-.946-.179l11.04 10.973zm0 2.067l-11 10.933c.298.036.612-.016.906-.183l13.324-7.54-3.23-3.21z"/>
      </svg>
      <div class="flex flex-col items-start">
        <span class="sm:inline hidden text-xs font-light">
          Coming Soon on
        </span>
        <span class="sm:hidden text-xs font-light">
          Soon on
        </span>
        <span class="sm:text-xl text-xs font-bold">
          Google Play
        </span>
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
