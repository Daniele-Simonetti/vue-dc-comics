<template>
  <div id="app">
    <Header />
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue"

export default {
  name: "App",
  components: {
    // HelloWorld,
    Header,
    // Main,
    // Footer,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss"
</style>
