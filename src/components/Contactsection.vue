<template>
  <section id="contact-section" class="text-center">
    <div class="container h-100">
      <div
        class="
          d-flex
          flex-column
          align-items-center
          justify-content-center
          h-100
        "
      >
        <h1 class="my-3">Want to work with us? Send a message</h1>
        <p class="my-3">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maiores
          cupiditate aliquid quis! Unde temporibus velit magni eius
          necessitatibus ad labore, tenetur asperiores placeat libero illo, sint
          ipsa pariatur rem quos?
        </p>
        <a href="#" class="btn contact-btn px-5 my-3">CONTACT</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Contactsection",
};
</script>

<style lang="scss">
@import "@/scss/_style.scss";
#contact-section {
  height: 450px;
  background-image: url(../assets/img/work-section-background-1.jpg);
  background-size: cover;
  p {
    color: $subtitle-grey;
  }
  .contact-btn {
    background-color: $main-color;
    border-radius: 0;
    &:hover {
      background-color: $rose;
      color: #fff;
    }
  }
}
</style>