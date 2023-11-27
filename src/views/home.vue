<template>
  <div class="home">
    <home-intro />
    <home-news />
    <slider />
  </div>
</template>

<script>
import HomeIntro from "@/components/home/home-intro.vue";
import HomeNews from "@/components/home/home-news.vue";
import Slider from "@/components/elements/slider.vue";

export default {
  name: "home",
  components: { HomeIntro, HomeNews, Slider },
};
</script>

<style lang="scss">
.home {
}
</style>
