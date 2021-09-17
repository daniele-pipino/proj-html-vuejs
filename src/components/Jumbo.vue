<template>
  <!-- start jumbo -->
  <div class="jumbo mx-3 mt-5" id="jumbo">
    <div class="container">
      <div class="row mb-5">
        <!-- left -->

        <div class="col-6 d-flex justify-content-end">
          <div class="col-2 d-flex align-items-center">
            <div
              class="
                chevron-bg
                d-flex
                justify-content-center
                align-items-center
                clickable
              "
            >
              <i
                @click="decreaseIndex"
                class="fas fa-chevron-left clickable fa-1x"
              ></i>
            </div>
          </div>
          <div class="col-10">
            <!-- title -->
            <h1 class="jumbo-title fw-light text-right mb-4">
              Devotion that never <span class="lobster">ends</span>
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
            <img
              v-for="(image, index) in images"
              :key="index"
              :src="getImages(image)"
              alt=""
              class="img-fluid"
              :class="currentIndex === index ? '' : 'd-none'"
            />
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
          <div class="col-2 d-flex align-items-center">
            <div
              class="
                chevron-bg
                d-flex
                justify-content-center
                align-items-center
                clickable
              "
            >
              <i @click="increaseIndex" class="fas fa-chevron-right"></i>
            </div>
          </div>
        </div>
        <!-- end col -->

        <!-- dot -->
        <div class="col-12 d-flex justify-content-center mt-5">
          <div
            v-for="(dot, dotIndex) in images"
            :key="dotIndex"
            class="dot mx-2 clickable"
            @click="setCurrentIndex(dotIndex)"
          ></div>
        </div>
      </div>
    </div>
  </div>
  <!-- end jumbo -->
</template>

<script>
export default {
  name: "Jumbo",
  data() {
    return {
      currentIndex: 0,
      images: ["jumbo-boys-1", "short-slider-rev-1-img-3", "slider-img-11"],
    };
  },
  created() {
    setInterval(() => {
      this.increaseIndex();
    }, 5000);
  },
  methods: {
    getImages(image) {
      return require(`@/assets/img/${image}.png`);
    },
    increaseIndex() {
      this.currentIndex++;
      if (this.currentIndex > this.images.length - 1) {
        this.currentIndex = 0;
      }
    },
    decreaseIndex() {
      this.currentIndex--;
      if (this.currentIndex < 0) {
        this.currentIndex = this.images.length - 1;
      }
    },
    setCurrentIndex(index) {
      return (this.currentIndex = index);
    },
  },
};
</script>

<style scoped lang="scss">
@import "@/scss/_style.scss";
.jumbo {
  .chevron-bg {
    width: 30px;
    height: 30px;
    background-color: $rose;
    border-radius: 50%;
  }
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
    &:hover {
      transform: scale(1.8);
    }
  }
}
</style>