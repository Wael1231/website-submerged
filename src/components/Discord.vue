<template>
  <div class="flex md:flex-row flex-col md:space-x-3 space-x-0 md:space-y-0 space-y-1 items-center justify-center sm:px-8 px-4 pb-6">
    <p class="text-white font-medium md:text-2xl sm:text-lg text-sm -mt-1">
      Play with
      <span v-if="memberCount > 0" class="font-black underline">
        {{ new Intl.NumberFormat().format(memberCount) }}
      </span>
      others on</p>
    <a href="https://discord.gg/polus"
       target="_blank"
       rel="noopener"
       class="block">
      <img class="object-contain sm:h-12 h-8 w-auto md:-mt-2 -mt-1"
           width="300"
           height="102"
           src="https://static.polus.gg/images/logos/discord/discord_logo_wordmark_white.svg"
           alt="Discord">
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
