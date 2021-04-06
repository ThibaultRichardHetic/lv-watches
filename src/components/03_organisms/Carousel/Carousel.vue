<template>
  <div class="container--carousel">
    <CpText tag="h3" type="hero-title ogg green">Collection</CpText>
    <VueSlickCarousel :arrows="true" :dots="true" v-bind="settings">
      <div v-for="slide in slides" :key="slide.title" class="slide">
        <div class="slide__img">
          <img :src="require(`@/assets/images/${ slide.img }`)" alt>
        </div>
        <div class="slide__content">
          <CpText type="description bold">{{ slide.title }}</CpText>
          <CpText type="slide">{{ slide.text }}</CpText>
          <a href class="button--plus">
            <CpText>Voir plus</CpText>
          </a>
        </div>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";

import CpText from "@/components/01_atoms/CpText/CpText.vue";

export default {
  name: "Carousel",
  components: {
    CpText,
    VueSlickCarousel
  },
  data() {
    return {
      text: "Louis vuitton test",
      settings: {
        dots: true,
        focusOnSelect: true,
        infinite: true,
        speed: 500,
        slidesToShow: 3,
        slidesToScroll: 3,
        touchThreshold: 5
      },
      slides: [
        {
          img: "watch-1.png",
          title: "#LVPRECOLL FALL 2020",
          text:
            "Louis Vuitton présente un cadran dédié à la précollection Homme Automne-Hiver 2020."
        },
        {
          img: "watch-2.png",
          title: "ESSENTIAL BROWN",
          text:
            "Offrez à votre montre le cadran brun iconique de l'horlogerie Louis Vuitton."
        },
        {
          img: "watch-3.png",
          title: "VALENTINE’S DAY 2021",
          text:
            "Cadran au motif Lovelygram ajoute une touche d'amour et de romance à la Saint-Valentin"
        },
        {
          img: "watch-3.png",
          title: "#LVPRECOLL FALL 2020",
          text:
            "Louis Vuitton présente un cadran dédié à la précollection Homme Automne-Hiver 2020."
        },
        {
          img: "watch-3.png",
          title: "#LVPRECOLL FALL 2020",
          text:
            "Louis Vuitton présente un cadran dédié à la précollection Homme Automne-Hiver 2020."
        }
      ]
    };
  }
};
</script>

<style lang="scss">
@import "./Carousel.scss";
</style>
