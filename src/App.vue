<template>
  <div id="app">
    <Header />
    <Main />
    <EndMain />
    <Footer />
    <EndFooter />
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import EndMain from "./components/EndMain.vue"
import Footer from "./components/Footer.vue"
import EndFooter from "./components/EndFooter.vue"


export default {
  name: "App",
  components: {
    // HelloWorld,
    Header,
    Main,
    EndMain,
    Footer,
    EndFooter,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss"
</style>
