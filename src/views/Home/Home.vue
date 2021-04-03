<template>
  <div class="home">
    <Header/>
  </div>
</template>

<script>

import Header from "@/components/03_organisms/Header/Header.vue";

export default {
  name: "Home",
  components: {
    Header
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
