<template>
  <footer>
    <div class="container h-100">
      <div
        class="row align-items-center justify-content-center h-100 text-center"
      >
        <!-- 1 -->
        <div class="col-3">
          <figure>
            <img src="@/assets/img/logo-sidearea-1.png" alt="logo" />
            <p class="fw-italic mt-3">Let's Get Creative</p>
          </figure>
        </div>
        <!-- 2 -->
        <div class="col-3">
          <p>maree.qode@gmail.com</p>
          <p>+ 44645 321 789</p>
        </div>
        <!-- 3 -->
        <div class="col-3">
          <p>Avenue d'Auderghem 10</p>
          <p>1040 Brusselles, Belgium</p>
        </div>
        <!-- 4 -->
        <div class="col-3">
          <p>Stay in touch with us</p>
          <div class="social d-flex justify-content-center">
            <p>
              <a href=""> <i class="fab fa-twitter mx-3"></i></a>
            </p>
            <p>
              <a href=""><i class="fab fa-pinterest-p mx-3"></i> </a>
            </p>
            <p>
              <a href=""> <i class="fab fa-facebook-f mx-3"></i></a>
            </p>
            <p>
              <a href=""><i class="fab fa-linkedin-in mx-3"></i> </a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss">
@import "@/scss/_style.scss";
footer {
  height: 200px;
  background-color: $main-color;
}
</style>