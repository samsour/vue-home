<template>
<div class="menu-button">
    <img class="menu-button__image" src="../assets/menu.svg">
</div>
</template>

<script>
export default {
  name: 'MenuButton'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.menu-button {
    width: 150px;
    height: 150px;
    background: #fff;
    display: flex;
    align-items: center;
    justify-content: center;

    &__image {
        width: 50px;
    }
}
</style>
