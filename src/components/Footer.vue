<template>
  <div class="nav-footer">
    <div class="w-70">
      <div class="listaSx">
        <div class="listaTop">
          <h2 class="h2">DC COMICS</h2>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Videos</li>
            <li>New</li>
          </ul>
        </div>
        <div class="listaBottom">
          <h2 class="h2">SHOP</h2>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
      </div>
      <div class="listaCentro">
        <h2 class="h2">DC</h2>
        <ul>
          <li>Terms of use</li>
          <li>Privacy policy (New)</li>
          <li>Ad Choices</li>
          <li>Adversting</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>
      <div class="listaDx">
        <h2 class="h2">SITES</h2>
        <ul>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.nav-footer {
  width: 100%;
  height: 400px;
  display: flex;
  align-items: center;
  background: #1f3346;
  background-image: url("../assets/img/dc-logo-bg.png"),
    url("../assets/img/footer-bg.jpg");
  background-position: 85% center, center;
  background-repeat: no-repeat;
  background-size: 30%, cover;
  .h2 {
    margin: 15px 0px;
    color: white;
    padding: 5px;
  }
  .w-70 {
    width: 70%;
    display: flex;
    margin: 0 auto;
  }
  .listaSx {
    margin-right: 20px;
    .listaTop {
      ul {
        li {
          list-style: none;
          color: grey;
          font-size: 14px;
          font-weight: 400;
          padding: 5px;
        }
      }
    }
    .listaBottom {
      ul {
        li {
          list-style: none;
          color: grey;
          font-size: 14px;
          font-weight: 400;
          padding: 5px;
        }
      }
    }
  }
  .listaCentro {
    margin: 0px 20px;
    ul {
      li {
        list-style: none;
        color: grey;
        font-size: 14px;
        font-weight: 400;
        padding: 5px;
      }
    }
  }
  .listaDx {
    margin-right: 20px;
    ul {
      li {
        list-style: none;
        color: grey;
        font-size: 14px;
        font-weight: 400;
        padding: 5px;
      }
    }
  }
}
</style>
