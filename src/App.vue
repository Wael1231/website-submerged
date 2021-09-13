<template>
  <div class="flex flex-col h-full">
    <div class="mb-auto lg:space-y-20 sm:space-y-14 space-y-8">
      <Navigation />
      <main class="lg:space-y-20 sm:space-y-14 space-y-8 pb-10">
        <Heading />
        <Downloads />
        <TownOfUs />
        <Discord />
      </main>
    </div>
    <Cliffs />
    <Legal />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Navigation from "./components/Navigation.vue";
import Heading from "./components/Heading.vue";
import Downloads from "./components/Downloads.vue";
import TownOfUs from "./components/TownOfUs.vue";
import Discord from "./components/Discord.vue";
import Cliffs from "./components/Cliffs.vue";
import Legal from "./components/Legal.vue";

export default defineComponent({
  name: "App",
  components: {
    Navigation,
    Heading,
    Downloads,
    TownOfUs,
    Discord,
    Cliffs,
    Legal,
  },
});
</script>

<style>
html, body {
  height: 100vh;
  background: linear-gradient(180deg, #1E0F35 0%, #000000 100%);
  background-attachment: fixed;
}

html {
  height: -webkit-fill-available;
}

body {
  min-height: 100vh;
  min-height: -webkit-fill-available;
}

#app {
  height: 100vh;
  width: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
