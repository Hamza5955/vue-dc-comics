<template>
  <div>
    <div class="jumbotron"></div>
  </div>
</template>

<script>
export default {
  name: "Maintop",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../Style/Variabili";
.jumbotron {
  width: 100%;
  height: 500px;
  display: flex;
  align-items: center;
  background: rgb(194, 6, 6);
  background-image: url("../assets/img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
