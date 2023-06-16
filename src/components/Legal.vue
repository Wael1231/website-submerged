<template>
  <div class="text-xs xs:text-sm sm:text-base pb-12 pt-6 pl-8 pr-8 xs:pl-10 xs:pr-10 sm:pl-28 sm:pr-28 text-purple-200 opacity-50 sm:space-y-6 space-y-4">
    <p>
      This mod is not affiliated with Among Us or Innersloth LLC, and the content contained therein is not endorsed or otherwise sponsored by Innersloth LLC.
      Portions of the materials contained herein are property of Innersloth LLC. &copy; Innersloth LLC.
    </p>
    <p>
      Submerged is licensed under a custom license. Please check LICENSE.md for more information in their github repo.
    </p>
    <p>
      &copy; {{ new Date().getFullYear() }} Submerged. All rights reserved.
    </p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Legal",
});
</script>
