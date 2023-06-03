<template>
  <div v-if="!mobile">
    <headerComponent/>
  </div>

  <div v-if="mobile">
    <MobileHeader />
  </div>


  <div>
    <img-carousel/>
  </div>

  <div v-if="!mobile">
    <card-loop>
      <cardActu/>
    </card-loop>
  </div>

  <div v-if="mobile">
    <cards-section/>

  </div>


  <title-banner/>

  <div v-if="mobile">
    <card-loop>
      <cardActu/>
    </card-loop>
  </div>

  <div v-if="!mobile">
    <cards-section/>

  </div>


  <footer-component/>
</template>

<script>
import headerComponent from "@/components/header";
import cardActu from "@/components/CardActu";
import ImgCarousel from "@/components/imgCarousel";
import TitleBanner from "@/components/titleBanner";
import CardsSection from "@/components/cardsSection";
import FooterComponent from "@/components/footerComponent";
import CardLoop from "@/components/CardLoop";
import MobileHeader from "@/components/MobileHeader";

export default {
  name: 'App',
  mobile: false,
  components: {
    CardLoop,
    FooterComponent,
    CardsSection,
    TitleBanner,
    ImgCarousel,
    headerComponent,
    cardActu,
    MobileHeader
  },

  beforeCreate() {
    this.mobile = document.documentElement.clientWidth <= 1024;

  }

}
</script>

<style>
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  margin: 0;
}
</style>
