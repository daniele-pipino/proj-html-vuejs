<template>
  <section id="blog-section" class="my-5">
    <div class="container">
      <div class="row justify-content-center">
        <!-- components -->
        <Blogcard v-for="(post, index) in blogpost" :key="index" :post="post" />
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
          title: "This way Loves, a detailed guide through new design",
          day: "07",
          month: "May'19",
          poster_path: "blog-img-1",
        },
        {
          id: 2,
          author: "By Emilie Fields",
          title: "I try to give people a different way of looking art",
          day: "07",
          month: "May'19",
          poster_path: "blog-img-2",
        },
        {
          id: 3,
          author: "By Emilie Fields",
          title: "Introduce Richrad Laperrière of those amazing features",
          day: "07",
          month: "May'19",
          poster_path: "blog-img-3",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>