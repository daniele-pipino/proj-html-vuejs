<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "scss/style.scss";
// utilities
.clickable {
  cursor: pointer;
}

#app {
  overflow-x: hidden;
}

.lobster {
  font-family: "Lobster", cursive;
}

.dancing-script {
  font-family: "Dancing Script", cursive;
}

a {
  color: black;
  &:hover {
    color: black;
  }
}
</style>
