<template>
  <div>
    <form action="get" class="form">
      <InputTitle v-for="input in inputs" :key="input.id" :input="input"/>
    </form>
    <ButtonText type="primary" :content="textButton"/>
  </div>
</template>

<script>

import InputTitle from "@/components/02_molecules/InputTitle/InputTitle.vue";
import ButtonText from "@/components/02_molecules/ButtonText/ButtonText.vue";

export default {
  name: "CpForm",
  components: {
    InputTitle,
    ButtonText
  },
  data() {
    return {
      h2: "Account",
      inputs: [["Email", "Jane.doe@gmail.com"], ["Full Name", "Jane Doe"]],
      textButton: "Save"
    };
  }
};
</script>

<style lang="scss">
  @import "./CpForm.scss";
</style>
