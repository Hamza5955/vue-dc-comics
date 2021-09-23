<template>
  <div>
    <div class="container">
      <div class="nero">
        <h2>Content goess here</h2>
      </div>
      <div class="blu">
        <div class="w-70">
          <li class="special" v-for="(icon, index) in specials" :key="index">
            <img :src="require(`../assets/img/${icon.img}`)" />
            <div class="nome">
              {{ icon.nome }}
            </div>
          </li>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import specials from "@/assets/data/Specials.js";
export default {
  name: "Main",
  data() {
    return { specials };
  },
};
</script>
<style scoped lang="scss">
.container {
  width: 100%;
  height: 300px;
  background-color: black;
}
.nero {
  display: flex;
  width: 90%;
  height: 150px;
  margin: 0 auto;
  color: white;
  align-items: center;
  flex-direction: row;
  margin-right: 50%;
}
.blu {
  display: flex;
  width: 100%;
  height: 150px;
  background-color: rgb(12, 77, 180);
  justify-content: space-around;
  align-items: center;
  list-style: none;
}
.blu > div {
  display: flex;
  flex-direction: row;
}
.resize {
  width: 30px;
}
.special {
  width: 50%;
}
.w-70 {
  flex-direction: row;
}
img {
  height: 70px;
}
.nome {
  color: azure;
}
</style>
