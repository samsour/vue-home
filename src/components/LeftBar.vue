<template>
<div class="left-bar">
    <MenuButton />
</div>
</template>

<script>
import MenuButton from '@/components/MenuButton.vue'

export default {
  name: 'leftBar',
  components: { MenuButton }
}
</script>

<style scoped lang="scss">
.left-bar {
  width: 50px;
  height: 100vh;
  display: flex;
  z-index: 1;
  align-content: flex-end;
}
</style>
