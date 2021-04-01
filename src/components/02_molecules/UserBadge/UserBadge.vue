<template>
  <div class="userbadge">
    <Avatar/>
    <CpText tag="p">{{ UserName }}</CpText>
  </div>
</template>

<script>
import Avatar from "@/components/01_atoms/Avatar/Avatar.vue";
import CpText from "@/components/01_atoms/CpText/CpText.vue";

export default {
  name: "UserBadge",
  components: {
    Avatar,
    CpText
  },
  data() {
    return {
      UserName: "Jane Doe"
    };
  }
};
</script>

<style lang="scss">
@import "UserBadge.scss";
</style>

