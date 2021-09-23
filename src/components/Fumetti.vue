<template>
  <div class="card">
    <img class="img-card" :src="it.thumb" alt="" />
    <div class="bianco">
      {{ it.series }}
    </div>
  </div>
</template>

<script>
export default {
  name: "Fumetti",
  props: ["it"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
  width: 15%;
  margin-top: 20px;
  margin-bottom: 20px;
}

.img-card {
  height: 150px;
  width: 150px;
}
.bianco {
  color: azure;
  padding: 10px 10px 10px 10px;
}
</style>
