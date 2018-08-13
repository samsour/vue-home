<template>
<div class="top-bar">
  <Logo name="Sam" surname="Sauer" user="sour" />
</div>
</template>

<script>
import Logo from "@/components/Logo.vue";

export default {
  name: "TopBar",
  components: { Logo }
};
</script>

<style scoped lang="scss">
.top-bar {
  background: #fff;
  height: 50px;
  z-index: 2;
}
</style>
