<template>
  <aside class="sidebar--account">
    <CpText tag="h2" type="subtitle">{{ h2 }}</CpText>
    <UserBadge/>
    <NavList />
    <ColorTheme />
  </aside>
</template>

<script>
import CpText from "@/components/01_atoms/CpText/CpText.vue";
import UserBadge from "@/components/02_molecules/UserBadge/UserBadge.vue"
import NavList from "@/components/02_molecules/NavList/NavList.vue"
import ColorTheme from "@/components/02_molecules/ColorTheme/ColorTheme.vue"

export default {
  name: "SidebarAccount",
  components: {
    CpText,
    UserBadge,
    NavList,
    ColorTheme
  },
  data() {
    return {
      h2: "Account"
    };
  }
};
</script>

<style lang="scss">
  @import "SidebarAccount.scss";
</style>
