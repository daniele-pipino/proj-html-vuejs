<template>
  <!-- start jumbo -->
  <div class="jumbo mx-3 mt-5">
    <div class="container">
      <div class="row mb-5">
        <!-- left -->

        <div class="col-6 d-flex justify-content-end">
          <div class="col-2">
            <!-- inserire icona -->
          </div>
          <div class="col-10">
            <!-- title -->
            <h1 class="jumbo-title fw-light text-right mb-4">
              Devotion that never ends
            </h1>
            <!-- subtitle -->
            <p class="jumbo-subtitle mb-5">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Magni
              qui corrupti enim error a eaque libero quisquam, natus vero
              deserunt explicabo numquam ab ad totam tenetur culpa minima
              consequuntur ipsa.
            </p>
            <!-- button -->
            <a href="#" class="btn jumbo-btn">READ MORE</a>
          </div>
        </div>

        <!-- right -->

        <div class="col-6 d-flex">
          <!-- left -->
          <div class="d-flex flex-column h-100 justify-content-between">
            <img
              src="@/assets/img/short-slider-rev-1-img-2.png"
              alt=""
              class="w-50 ms-5"
            />
            <img
              src="@/assets/img/short-slider-rev-1-img-10.png"
              alt=""
              class="w-50"
            />
            <img
              src="@/assets/img/short-slider-rev-1-img-8.png"
              alt=""
              class="w-50 ms-4"
            />
          </div>
          <!-- center -->
          <div class="d-flex">
            <img src="@/assets/img/jumbogirl.png" alt="" class="w-50" />
            <img src="@/assets/img/jumbo-boy.png" alt="" class="w-50 ms-1" />
          </div>
          <!-- right -->
          <div class="d-flex flex-column h-100 justify-content-between">
            <img
              src="@/assets/img/slider-img-14.png"
              alt=""
              class="w-50 me-5"
            />
            <img
              src="@/assets/img/short-slider-rev-1-img-6.png"
              alt=""
              class="w-50"
            />
            <img
              src="@/assets/img/slider-img-17.png"
              alt=""
              class="w-50 me-4"
            />
          </div>
          <div class="col-1">
            <!-- inserire icona -->
          </div>
        </div>
        <!-- end col -->
        <div class="col-12 d-flex justify-content-center mt-5">
          <div class="dot mx-2 clickable"></div>
          <div class="dot mx-2 clickable"></div>
          <div class="dot mx-2 clickable"></div>
        </div>
      </div>
    </div>
  </div>
  <!-- end jumbo -->
</template>

<script>
export default {
  name: "Jumbo",
};
</script>

<style scoped lang="scss">
@import "@/scss/_style.scss";
.jumbo {
  .jumbo-title {
    font-size: 75px;
  }
  .jumbo-subtitle {
    color: $subtitle-grey;
  }
  .jumbo-btn {
    border: 2px solid $rose;
    border-radius: 0;
    padding: 7px 18px;
    &:hover {
      background-color: $rose;
    }
  }
  .dot {
    border-radius: 50%;
    padding: 3px;
    width: 10px;
    height: 10px;
    background-color: $rose;
  }
}
</style>