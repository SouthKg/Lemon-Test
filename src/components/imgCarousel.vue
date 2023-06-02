<template>
  <div class="slider-container">
    <div class="menu">
      <label for="slide-dot-1"></label>
      <label for="slide-dot-2"></label>
      <label for="slide-dot-3"></label>
    </div>

    <div class="slide">
      <input class="slide-input" id="slide-dot-1" type="radio" name="slides" checked>
      <img class="slide-img" src="../assets/img-carousel.png">
      <div class="slide-text">
        <h2>Titre de la diapositive 1</h2>
        <p>Description de la diapositive 1</p>
      </div>
    </div>

    <div class="slide">
      <input class="slide-input" id="slide-dot-2" type="radio" name="slides">
      <img class="slide-img" src="../assets/img-carousel.png">
      <div class="slide-text">
        <h2>Titre de la diapositive 2</h2>
        <p>Description de la diapositive 2</p>
      </div>
    </div>

    <div class="slide">
      <input class="slide-input" id="slide-dot-3" type="radio" name="slides">
      <img class="slide-img" src="../assets/img-carousel.png">
      <div class="slide-text">
        <h2>Titre de la diapositive 3</h2>
        <p>Description de la diapositive 3</p>
      </div>
    </div>
  </div>


</template>

<script>
export default {
  name: "imgCarousel"
}
</script>

<style scoped>html, body {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
}
img {
  max-width: 100%;
}
.slider-container {
  width:100%;
  position: relative;
  margin: auto;
  height: 500px;
  overflow: hidden;
}
.menu {
  position: absolute;
  left: 0;
  z-index: 999;
  width: 100%;
  bottom: 0;
  text-align: center;
}
.menu label {
  cursor: pointer;
  display: inline-block;
  width: 45px;
  height: 5px;
  background: #FFFFFF80;
  border-radius: 0;
  margin: 0 0.2em 1em;
}
.menu label:hover,.menu label:focus {
  background: white;
}
.slide-input{
  opacity: 0;
}
.slide-img {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 100%;
  z-index: 10;
  transition: left 0s 0.75s;
}
[id^="slide"]:checked + .slide-img {
  left: 0;
  z-index: 100;
  transition: left 0.65s ease-out;
}
.slide-text{
  z-index: 999;
  position:relative;
}
.slide-text {
  display: none;
  position: absolute;
  top: 75%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  text-align: center;
}

.slide-input:checked + .slide-img + .slide-text {
  display: block;
}

@media screen and (max-width:1024px){
  .slider-container[data-v-c9bcd23a] {
    height: 145px;
  }
  .slide-text{
    display:none !important;
  }
}

</style>