<template>
<div>
  <h2>
    Le futur passe par l'écologie
  </h2>
</div>
</template>

<script>
export default {
  name: "titleBanner"
}
</script>

<style scoped>
  div{
    background-image: url("../assets/background-ecologie.png");
    height:200px;
    display:flex;
    justify-content:center;
    align-items: center;
  }
  h2{
    color:white;
    background:#0E3706B5;
    padding:15px 30px;
    border-radius: 30px;

    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 28px;
    line-height: 34px;
  }

  @media screen and (max-width:1024px){
    h2{
      font-size:21px;
    }
  }
</style>