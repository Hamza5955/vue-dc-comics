<template>
  <div>
    <div class="container">
      <div class="nero">
        <h2>Content goess here</h2>
      </div>
      <div class="blu">
        <div>
          <img
            class="resize"
            src="../assets/img/buy-comics-digital-comics.png"
            alt="vue-test\src\assets\img"
          />
          <div>digital comics</div>
        </div>
        <div>
          <img
            class="resize"
            src="..\assets\img\buy-comics-digital-comics.png"
            alt=""
          />
          <div>dc merchandise</div>
        </div>
        <div>
          <img
            class="resize"
            src="..\assets\img\buy-comics-digital-comics.png"
            alt=""
          />
          <div>subscription</div>
        </div>
        <div>
          <img
            class="resize"
            src="..\assets\img\buy-comics-digital-comics.png"
            alt=""
          />
          <div>comic shop locator</div>
        </div>
        <div>
          <img
            class="resize"
            src="..\assets\img\buy-comics-digital-comics.png"
            alt=""
          />
          <div>dc power visa</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
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
}
.blu {
  display: flex;
  width: 100%;
  height: 150px;
  background-color: rgb(12, 77, 180);
  justify-content: space-around;
  align-items: center;
}
.blu > div {
  display: flex;
  flex-direction: row;
}
.resize {
  width: 30px;
}
</style>
