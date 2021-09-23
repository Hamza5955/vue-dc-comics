<template>
  <div class="icon-footer">
    <div class="w-70">
      <div class="sing-up">
        <h3 class="up">SING-UP NEW!</h3>
      </div>
      <div class="follow">
        <h3 class="us">FOLLOW US</h3>
        <li class="social" v-for="(icon, index) in socials" :key="index">
          <img :src="require(`../assets/img/footer${icon.img}`)" alt="" />
        </li>
      </div>
    </div>
  </div>
</template>

<script>
import Socials from "@/assets/data/Socials.js";
export default {
  name: "FooterB",
  data() {
    return {
      socials: Socials,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../Style/Variabili";
.icon-footer {
  width: 100%;
  height: 140px;
  align-items: center;
  background: #363535;
  .w-70 {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
    width: 70%;
    display: flex;
    margin: 0 auto;
    .sing-up {
      border: 2px solid #077cea;
      padding: 20px;
      .up {
        color: white;
      }
    }
    .follow {
      display: flex;
      align-items: center;
      .us {
        color: #077cea;
        margin-right: 15px;
      }
      li {
        list-style: none;
        padding: 10px;
      }
    }
  }
}
</style>
