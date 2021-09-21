<template>
  <footer>
    <div class="container">
      <div
        v-for="(link, index) in footerlinks"
        :key="index"
        :class="link.title ? 'active' : null"
      >
        {{ link.text }}
      </div>
    </div>
  </footer>
</template>

<script>
import * as footerlinks from "../assets/data/footerlinks.js";
export default {
  name: "Footer",
  data() {
    return { footerlinks: footerlinks.footerlinks };
  },
};
</script>
<style scoped lang="scss">
.container {
  width: 100%;
  height: 400px;
  background-color: yellow;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
}
.active {
  color: aqua;
}
</style>
