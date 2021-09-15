<template>
  <section id="square-section">
    <div class="row">
      <!-- 1 -->
      <div class="col-4 p-0">
        <img src="@/assets/img/port-img-1.jpg" alt="" class="img-fluid" />
      </div>
      <!-- 2 -->
      <div class="col-4 p-0">
        <img src="@/assets/img/port-img-2.jpg" alt="" class="img-fluid" />
      </div>
      <!-- 2 -->
      <div class="col-4 p-0">
        <img src="@/assets/img/port-img-3.jpg" alt="" class="img-fluid" />
      </div>
      <!-- 4 -->
      <div class="col-4 p-0 book-column clickable">
        <img src="@/assets/img/port-img-4.jpg" alt="" class="img-fluid img-1" />
      </div>
      <!-- 5 -->
      <div class="col-4 p-0">
        <img src="@/assets/img/port-img-5.jpg" alt="" class="img-fluid" />
      </div>
      <!-- 6 -->
      <div class="col-4 p-0">
        <img src="@/assets/img/port-img-6.jpg" alt="" class="img-fluid" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Squaresection",
};
</script>

<style scoped lang="scss">
.book-column {
  background-image: url("../assets/img/hover-book.png");
  background-size: cover;
  .img-1 {
    &:hover {
      opacity: 0;
    }
  }
}
</style>