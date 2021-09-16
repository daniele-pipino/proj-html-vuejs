<template>
  <section id="blog-section" class="my-5">
    <div class="container">
      <div class="row">
        <Blogcard />
      </div>
    </div>
  </section>
</template>

<script>
import Blogcard from "@/components/Blogcard.vue";
export default {
  name: "Blogsection",
  components: {
    Blogcard,
  },
  data() {
    return {
      blogpost: [
        {
          id: 1,
          author: "By Emilie Fields",
          title: "",
          day: "",
          month: "",
          poster_path: "",
        },
        {
          id: 2,
          author: "By Emilie Fields",
          title: "",
          day: "",
          month: "",
          poster_path: "",
        },
        {
          id: 3,
          author: "By Emilie Fields",
          title: "",
          day: "",
          month: "",
          poster_path: "",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>