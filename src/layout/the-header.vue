<template>
  <header class="the-header">
    the-header

    <!-- <v-layout>
      <v-app-bar color="primary" prominent>
        <v-app-bar-nav-icon
          variant="text"
          @click.stop="drawer = !drawer"
        ></v-app-bar-nav-icon>

        <v-spacer></v-spacer>
      </v-app-bar>

      <v-navigation-drawer v-model="drawer" location="bottom" temporary>
        <v-list :items="items"></v-list>
      </v-navigation-drawer>

      <v-main>
        <v-container class="">
          <v-img
            class="the-header__image"
            src="../../public/assets/header/header-logo.svg"
          />

          <v-text-field
            class="mt-5"
            hide-details
            label="Поиск по сайту"
            variant="outlined"
          ></v-text-field>
          <div class="d-flex mt-5">
            <v-btn class="mx-auto">Поступить</v-btn>
          </div>
        </v-container>
      </v-main>
    </v-layout> -->
  </header>
</template>

<script>
export default {
  name: "the-header",
  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: "Значение 1",
        value: "Значение 1",
      },
      {
        title: "Значение 2",
        value: "Значение 2",
      },
      {
        title: "Значение 3",
        value: "Значение 3",
      },
      {
        title: "Значение 4",
        value: "Значение 4",
      },
    ],
  }),
  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>

<style lang="scss">
.the-header {
  &__image {
    max-width: 200px !important;
    margin: 0 auto;
  }
}
</style>
