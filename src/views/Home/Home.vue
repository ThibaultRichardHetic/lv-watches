<template>
  <div class="home">
    <Header/>
    <Hero/>
    <Articles />
    <Carousel />
    <Media />
    <Footer />
  </div>
</template>

<script>

import Header from "@/components/03_organisms/Header/Header.vue";
import Hero from "@/components/03_organisms/Hero/Hero.vue";
import Articles from "@/components/03_organisms/Articles/Articles.vue";
import Carousel from "@/components/03_organisms/Carousel/Carousel.vue";
import Media from "@/components/03_organisms/Media/Media.vue";
import Footer from "@/components/03_organisms/Footer/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Hero,
    Articles,
    Carousel,
    Media,
    Footer
  },
  data() {
    return {
      text: "Louis vuitton test"
    };
  }
};
</script>

<style lang="scss">
@import "./Home.scss"
</style>
