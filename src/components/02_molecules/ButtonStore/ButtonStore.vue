<template>
  <div :class="`container--button-store ${color}`">
    <CpLink>
      <div class="container--illu">
        <img v-if="brand == 'apple'" src="@/assets/images/apple.svg" alt>
        <img v-if="brand == 'android'" src="@/assets/images/android.svg" alt>
      </div>
      <div class="container--text">
        <CpText type="button-m">Get it for</CpText>
        <CpText v-if="brand == 'apple'" type="button-m brand">IOS</CpText>
        <CpText v-if="brand == 'android'" type="button-m brand">Android</CpText>
      </div>
    </CpLink>
  </div>
</template>

<script>
import CpText from "@/components/01_atoms/CpText/CpText.vue";
import CpLink from "@/components/01_atoms/CpLink/CpLink.vue";

export default {
  name: "ButtonStore",
  props: {
    brand: {
      type: String,
      default: "apple"
    },
    color: {
      type: String,
      default: "light"
    }
  },
  components: {
    CpText,
    CpLink
  }
};
</script>

<style lang="scss">
@import "./ButtonStore.scss";
</style>
