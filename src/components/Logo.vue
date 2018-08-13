<template>
    <div class="logo">
        <div class="logo__text">
            <div class="logo__text__surname">
              {{name}}
            </div>
            <div class="logo__text__name">
                <vue-typer :text='["sour","Sauer"]' erase-style='backspace'></vue-typer>
            </div>
        </div>
     </div>
</template>

<script>
import { VueTyper } from "vue-typer";

export default {
  name: "Logo",
  components: {
    VueTyper
  },
  props: {
    user: String,
    name: String,
    surname: String
  },
  methods: {},
  mounted: function() {
    this.$nextTick(function() {
      // rendered
    });
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.logo {
  width: 150px;
  height: 150px;
  background: #fff;
  display: grid;
  align-items: center;
  justify-content: center;

  &__text {
    font-family: "Podkova", serif;
    font-size: 24px;
    min-width: 63px;
    &__surname {
      font-weight: bold;
    }
    // &__name {
    //   &::after {
    //     content: "_";
    //     margin-left: -4px;
    //   }
    // }
  }
}
</style>
