<template>
  <div class="navlist">
    <ul>
      <li v-for="element in elements" :key="element.id">
        <NavElement :elText="element"/>
      </li>
    </ul>
  </div>
</template>

<script>
import NavElement from "@/components/02_molecules/NavElement/NavElement.vue";

export default {
  name: "NavList",
  components: {
    NavElement
  },
  data() {
    return {
      elements: ["Profile", "Settings", "Data"]
    };
  }
};
</script>

<style lang="scss">
@import "NavList.scss";
</style>

