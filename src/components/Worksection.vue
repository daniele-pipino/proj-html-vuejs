<template>
  <section id="work-section" class="my-5">
    <div class="container">
      <div class="text-center">
        <!-- title -->
        <h1 class="m-5">Working Process</h1>
        <!-- process -->
        <div class="process-container d-flex justify-content-center">
          <div v-for="(work, index) in workProcess" :key="index" class="m-4">
            <div class="d-flex flex-column align-items-center proces-col">
              <div class="bg-rounded">
                <i :class="work.icon"></i>
              </div>

              <h4 class="mt-3">{{ work.name }}</h4>
              <p class="mt-3">{{ work.explanation }}</p>
            </div>
          </div>
          <!-- end process-->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Worksection",
  data() {
    return {
      workProcess: [
        {
          id: 1,
          icon: "fas fa-lightbulb fa-2x icon-green",
          name: "First there is an idea",
          explanation:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sint ullam minus, eaque porro placeat dolores consequatur impedit.",
        },
        {
          id: 2,
          icon: "far fa-comment fa-2x icon-yellow",
          name: "Then we talk about",
          explanation:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sint ullam minus, eaque porro placeat dolores consequatur impedit.",
        },
        {
          id: 3,
          icon: "fas fa-cloud fa-2x icon-violet",
          name: "And we Think About",
          explanation:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sint ullam minus, eaque porro placeat dolores consequatur impedit.",
        },
        {
          id: 1,
          icon: "fas fa-pencil-alt fa-2x icon-red",
          name: "So we draw along",
          explanation:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sint ullam minus, eaque porro placeat dolores consequatur impedit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" >
@import "@/scss/_style.scss";
#work-section {
  .process-container {
    background-image: url("../assets/svg/svg-3.svg");
    background-repeat: no-repeat;
    background-position: top;
  }
  .bg-rounded {
    border-radius: 50%;
    background-color: $antique-color;
    width: 110px;
    height: 110px;
    position: relative;
    i {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    // icon color
    .icon-green {
      color: $green-apple;
    }
    .icon-yellow {
      color: $lemon;
    }
    .icon-violet {
      color: $my-violet;
    }
    .icon-red {
      color: $brick;
    }
  }
}
</style>