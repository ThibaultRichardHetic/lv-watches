<template>
  <div class="inputtitle">
    <CpText tag="h4">{{ input[0] }}</CpText>
    <CpInput :placeholder="input[1]"/>
  </div>
</template>

<script>

import CpText from "@/components/01_atoms/CpText/CpText.vue";
import CpInput from "@/components/01_atoms/CpInput/CpInput.vue";


export default {
  name: "InputTitle",
  components: {
    CpText,
    CpInput
  },
  props: ['input'],
  data() {
    return {
    };
  }
};
</script>

<style lang="scss">
@import "./InputTitle.scss";
</style>
