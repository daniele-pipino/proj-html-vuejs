<template>
  <main>
    <Squaresection />
    <Worksection />
  </main>
</template>

<script>
import Squaresection from "@/components/Squaresection.vue";
import Worksection from "@/components/Worksection.vue";
export default {
  name: "Main",
  components: {
    Squaresection,
    Worksection,
  },
};
</script>

<style lang="scss">
@import "@/scss/_variables.scss";
</style>