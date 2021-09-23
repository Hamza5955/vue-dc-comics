<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
    <Footerb />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Footerb from "./components/Footerb.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
    Footerb,
  },
};
</script>

<style lang="scss">
@import "@/style/general.scss";
#app {
}
</style>
