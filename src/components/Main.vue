<template>
  <main>
    <Squaresection />
    <Worksection />
    <Contactsection />
    <Blogsection />
  </main>
</template>

<script>
import Squaresection from "@/components/Squaresection.vue";
import Worksection from "@/components/Worksection.vue";
import Contactsection from "@/components/Contactsection.vue";
import Blogsection from "@/components/Blogsection.vue";
export default {
  name: "Main",
  components: {
    Squaresection,
    Worksection,
    Contactsection,
    Blogsection,
  },
};
</script>

<style lang="scss">
</style>