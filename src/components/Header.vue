<template>
  <div>
    <Navbar />
    <Jumbo />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Jumbo from "@/components/Jumbo.vue";
export default {
  name: "Header",
  components: {
    Navbar,
    Jumbo,
  },
};
</script>

<style lang="scss" scoped>
</style>