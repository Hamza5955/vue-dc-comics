<template>
  <header>
    <div class="header-nav container">
      <div class="logo">
        <a href="/"><img src="@/assets/img/dc-logo.png" alt=""/></a>
      </div>
      <div class="nav-menu">
        <ul class="nav-it">
          <li
            v-for="(link, index) in links"
            :key="index"
            class="nav-item"
            :class="link.current ? 'active' : null"
          >
            <a :href="link.url">{{ link.text.toUpperCase() }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
import Links from "@/assets/data/Links.js";
export default {
  name: "Header",
  data() {
    return {
      links: Links.headerLinks,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/general";
.header-nav {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 4px solid transparent;
}
.logo {
  width: 80px;
  img {
    width: 100%;
  }
}
.nav-menu {
  height: 100%;
}
.nav-it {
  list-style: none;
  display: flex;
  font-size: 13px;
  font-weight: 550;
  line-height: 100px;
}
.nav-item {
  padding: 0px 15px;
  color: $secondary-color;
  a {
    text-decoration: none;
    color: inherit;
    &:hover {
      color: $primary-color;
    }
  }
}
</style>
