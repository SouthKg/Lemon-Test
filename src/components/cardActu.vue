<template>
  <div class="card-actu">
    <img src="https://picsum.photos/200/300">
    <h2>title card</h2>
    <p>Lorem ipsum...</p>
    <div class="row">
      <div class="column"><i class="fas fa-calendar"></i> 01/06/2023</div>
      <div class="column"><button class="see-more">En savoir plus</button></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardActu"
}
</script>

<style scoped>
  .card-actu{
    border : solid 1px black;
  }
</style>