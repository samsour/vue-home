<template>
  <div id="app">
    <top-bar/>
    <router-view/>
    <!-- <full-page ref="fullpage" :options="options" id="fullpage">
    <div class="section">
      First section ...
    </div>
    <div class="section">
      Second section ...
    </div>
  </full-page> -->
  </div>
</template>

<script>
// @ is an alias to /src
import TopBar from "@/components/TopBar.vue";

export default {
  name: "app",
  components: {
    TopBar
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Podkova|Open+Sans");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Open Sans", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #111;
  background: #eee;
  height: 100vh;
}
</style>
