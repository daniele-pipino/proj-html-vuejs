<template>
  <div class="col-4 mt-5">
    <!-- image -->
    <figure class="position-relative">
      <img src="@/assets/img/blog-img-1.jpg" alt="" class="img-fluid" />
      <div class="article-date">
        <div class="day text-center"></div>
        <div class="month-year"></div>
      </div>
    </figure>
    <!-- end image -->
    <h4>Ciao sono bello ciao ciao ciao ciao</h4>
    <p class="fw-italic">By Emilie fields</p>
  </div>
</template>

<script>
export default {
  name: "Blogcard",
};
</script>

<style lang="scss">
@import "@/scss/_style.scss";
.article-date {
  .day {
    width: 50px;
    height: 40px;
    background-color: $green-apple;
    position: absolute;
    top: -15px;
    left: 15px;
  }
  .month-year {
    width: 50px;
    min-height: 40px;
    background-color: $rose;
    position: absolute;
    top: 25px;
    left: 15px;
  }
}
</style>