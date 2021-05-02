<template>
  <div class="flex flex-wrap items-center justify-center sm:px-8 px-4 pb-6">
    <p class="text-white font-medium md:text-2xl sm:text-lg text-sm mr-2 -mt-1">
      Play with
      <span v-if="memberCount > 0" class="font-black underline">{{ new Intl.NumberFormat().format(memberCount) }}</span>
      others &amp; stay up to date on</p>
    <a href="https://discord.gg/polus" target="_blank" class="block">
      <img class="object-contain sm:h-14 h-8" alt="Discord logo" src="https://static.polus.gg/images/logos/discord/discord_white.svg">
    </a>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Discord",
  data() {
    return {
      memberCount: 0,
    };
  },
  beforeMount() {
    this.getMemberCount();
  },
  methods: {
    async getMemberCount() {
      try {
        const res = await fetch("https://discord.com/api/v8/invites/polus?with_counts=true");
        const data = await res.json();

        this.memberCount = data["approximate_member_count"] ?? 0;
      } catch (error) {
        console.error("Error fetching Discord invite details", error);
      }
    },
  },
});
</script>
