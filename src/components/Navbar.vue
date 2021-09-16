<template>
  <div>
    <header class="d-flex justify-content-between mx-4" id="Navbar">
      <!-- logo -->
      <div class="logo pt-3">
        <a href="#Navbar"
          ><img src="@/assets/img/logo-sidearea-1.png" alt="" class="img-fluid"
        /></a>
      </div>
      <!-- navbar -->
      <div class="nav-bar d-flex">
        <ul class="d-flex align-items-center justify-content-center pt-2">
          <li v-for="(item, index) in navbar" :key="index" class="mx-3 fw-bold">
            <a href="#">{{ item.element }}</a>
          </li>
          <li class="mx-3 fw-bold">
            <a href="#"
              ><img
                src="@/assets/svg/svg-1.svg"
                alt="dot.menu"
                class="dot-menu pb-1"
            /></a>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      navbar: [
        {
          element: "HOME",
        },
        {
          element: "PAGES",
        },
        {
          element: "PORTFOLIO",
        },
        {
          element: "BLOG",
        },
        {
          element: "SHOP",
        },
        {
          element: "ELEMENTS",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/scss/_variables.scss";
header {
  height: 70px;
  .nav-bar {
    ul li {
      list-style-type: none;
    }
    a {
      text-transform: uppercase;
      text-decoration: none;
      color: $link-color;
      font-size: 13px;
      line-height: 70px;
    }
    .dot-menu {
      width: 20px;
    }
  }
}
</style>