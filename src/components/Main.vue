<template>
  <main>
    <Squaresection />
    <Worksection />
    <Contactsection />
  </main>
</template>

<script>
import Squaresection from "@/components/Squaresection.vue";
import Worksection from "@/components/Worksection.vue";
import Contactsection from "@/components/Contactsection.vue";
export default {
  name: "Main",
  components: {
    Squaresection,
    Worksection,
    Contactsection,
  },
};
</script>

<style lang="scss">
@import "@/scss/_variables.scss";
</style>