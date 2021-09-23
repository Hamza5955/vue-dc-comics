<template>
  <div id="app">
    <Header />

    <Maintop />
    <Headerbotom />
    <Main />
    <Footer />
    <Footerb />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Maintop from "./components/Maintop.vue";
import Headerbotom from "./components/Headerbotom.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Footerb from "./components/Footerb.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Headerbotom,
    Footer,
    Footerb,
    Maintop,
  },
};
</script>

<style lang="scss">
@import "@/style/general.scss";
#app {
}
</style>
