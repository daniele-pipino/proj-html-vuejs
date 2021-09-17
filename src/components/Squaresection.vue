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
      <!-- 3 -->
      <div class="col-4 p-0 position-relative">
        <img src="@/assets/img/port-img-3.jpg" alt="" class="img-fluid" />
        <!-- right icons -->
        <div class="object">
          <!-- 1 -->
          <div class="recharge d-flex justify-content-center clickable">
            <img src="@/assets/svg/circle.svg" alt="" class="w-50" />
          </div>
          <!-- 2 -->
          <div class="shop d-flex justify-content-center mt-1 clickable">
            <img src="@/assets/svg/svg-6.svg" alt="" class="w-50" />
          </div>
        </div>
        <!-- end icons -->
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
      <div class="col-4 p-0 position-relative">
        <img src="@/assets/img/port-img-6.jpg" alt="" class="img-fluid" />
        <!-- arrow -->
        <div
          class="
            arrow-up
            clcikable
            d-flex
            justify-content-center
            align-items-center
          "
        >
          <a href="#header"
            ><img src="@/assets/svg/arrow-up.svg" alt="" class=""
          /></a>
        </div>
        <!-- end arrow  -->
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Squaresection",
};
</script>

<style lang="scss">
@import "@/scss/_variables.scss";
#square-section {
  .object {
    // container
    width: 40px;
    position: absolute;
    top: 90px;
    right: 0;

    // elements
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    .recharge,
    .shop {
      height: 30px;
      width: 30px;
    }
    .recharge {
      background-color: $rubin;
    }
    .shop {
      background-color: $white;
    }
  }
  // book col
  .book-column {
    background-image: url("../assets/img/hover-book.png");
    background-size: cover;
    .img-1 {
      &:hover {
        opacity: 0;
      }
    }
  }
  // freccia
  .arrow-up {
    height: 35px;
    width: 35px;
    background-color: $main-color;
    position: fixed;
    bottom: 20px;
    right: 15px;
  }
}
</style>