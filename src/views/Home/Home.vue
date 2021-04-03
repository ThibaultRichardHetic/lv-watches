<template>
  <div class="home">
    <Header/>
    <Hero/>
  </div>
</template>

<script>

import Header from "@/components/03_organisms/Header/Header.vue";
import Hero from "@/components/03_organisms/Hero/Hero.vue";

export default {
  name: "Home",
  components: {
    Header,
    Hero
  },
  data() {
    return {
      text: "Louis vuitton test"
    };
  }
};
</script>

<style lang="scss">
@import "./Home.scss"
</style>
