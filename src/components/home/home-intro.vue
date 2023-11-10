<template>
  <section class="home-intro">
    <div
      class="home-intro__grayscale d-flex flex-column justify-center align-center"
    >
      <h1 class="home-intro__grayscale-title h1 text-center color-white">
        ХТУ - верная траектория вашего обучения
      </h1>
      <v-btn class="home-intro__grayscale-button mt-5">История ВУЗа</v-btn>
    </div>
  </section>
</template>

<script>
export default {
  name: "home-intro",
};
</script>

<style lang="scss">
.home-intro {
  min-height: 300px;
  background-image: url(../../../public/assets/home/home-intro-background.jpg);
  background-size: cover;
  background-position: center center;

  &__grayscale {
    min-height: 300px;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.4);

    &-button {
      max-width: 255px !important;
      width: 100% !important;
      height: 48px !important;
      box-shadow: none !important;
      border: 2px solid $white !important;
      background-color: transparent !important;
      border-radius: 0 !important;

      &:hover {
        box-shadow: none !important;
        border-color: $main-blue !important;
        background-color: $white !important;

        & .v-btn__content {
          color: $main-blue;
        }
      }

      & .v-btn__content {
        color: $white;
      }
    }
  }
}
</style>
