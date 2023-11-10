<template>
  <div class="home">
    <home-intro />
    <home-news />
  </div>
</template>

<script>
import HomeIntro from "@/components/home/home-intro.vue";
import HomeNews from "@/components/home/home-news.vue";

export default {
  name: "home",
  components: { HomeIntro, HomeNews },
};
</script>

<style lang="scss">
.home {
}
</style>
