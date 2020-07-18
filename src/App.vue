<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({})
export default class App extends Vue {}
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Montserrat:400,500,600,700&display=swap");
@import url("./assets/font/iconfont.css");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  flex-shrink: 0;
  flex-grow: 0;
}

html,
body {
  background-color: #1e2125;
}

#app {
  position: absolute;
  width: 100%;
  height: 100%;
  min-width: 600px;
  min-height: 600px;

  background-color: #1e2125;
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
