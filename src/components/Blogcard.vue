<template>
  <div class="col-3 mt-5 clickable">
    <!-- image -->
    <figure class="position-relative">
      <img :src="getPoster(this.post.poster_path)" alt="" class="img-fluid" />
      <div class="article-date">
        <!-- date -->
        <div
          class="
            day
            d-flex
            justify-content-center
            align-items-center
            lobster
            fs-3
          "
        >
          <div>
            {{ post.day }}
          </div>
        </div>
        <!-- month -->
        <div
          class="
            month-year
            text-center
            fw-bold
            d-flex
            align-items-center
            justify-content-center
          "
        >
          {{ post.month }}
        </div>
      </div>
    </figure>
    <!-- end image -->
    <h5 class="fw-light mb-3">{{ post.title }}</h5>
    <p class="fst-italic dancing-script">{{ post.author }}</p>
  </div>
</template>

<script>
export default {
  name: "Blogcard",
  props: ["post"],
  data() {
    return {};
  },
  methods: {
    getPoster(poster) {
      return require(`@/assets/img/${poster}.jpg`);
    },
  },
};
</script>

<style lang="scss">
@import "@/scss/_style.scss";

.article-date {
  .day {
    width: 50px;
    height: 40px;
    background-color: $main-color;
    position: absolute;
    top: -15px;
    left: 15px;
    padding-top: 7px;
  }
  .month-year {
    width: 50px;
    min-height: 30px;
    background-color: $rose;
    position: absolute;
    top: 25px;
    left: 15px;
    font-size: 12px;
    padding-top: 7px;
  }
}
</style>