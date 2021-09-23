<template>
  <div class="barra">
    <div class="barra-nera">
      <Fumetti v-for="(item, index) in fumetti" :key="index" :it="item" />
    </div>
  </div>
</template>

<script>
import Fumetti from "@/components/Fumetti.vue";
import fumeti from "@/assets/data/fumeti.js";
export default {
  name: "Main",
  components: {
    Fumetti,
  },
  data() {
    return {
      fumetti: fumeti,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
//@import "../components/Style/Variabili";
.barra {
  width: 100%;
  display: flex;
  align-items: center;
  background: black;
  .barra-nera {
    width: 70%;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    background: rgb(24, 24, 24);
  }
}
img {
  height: 10000px;
}
</style>
