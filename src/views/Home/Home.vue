<template>
  <div class="home">
    <CpText tag="h1" type="">{{ text }}</CpText>
  </div>
</template>

<script>

import CpText from "@/components/01_atoms/CpText/CpText.vue";

export default {
  name: "Home",
  components: {
    CpText
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
