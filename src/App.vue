<template>
  <headerComponent />
  <div>
    <img-carousel />
  </div>
  <card-loop>
    <cardActu />
  </card-loop>

  <title-banner />
  <cards-section />
  <footer-component />
</template>

<script>
import headerComponent from "@/components/header";
import cardActu from "@/components/CardActu";
import ImgCarousel from "@/components/imgCarousel";
import TitleBanner from "@/components/titleBanner";
import CardsSection from "@/components/cardsSection";
import FooterComponent from "@/components/footerComponent";
import CardLoop from "@/components/CardLoop";

export default {
  name: 'App',
  components: {
    CardLoop,
    FooterComponent,
    CardsSection,
    TitleBanner,
    ImgCarousel,
    headerComponent,
    cardActu
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body{
  margin:0;
}
</style>
