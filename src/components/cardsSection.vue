<template>
  <div class="row">
    <div class="column">
      <h3>Inter quos eminebat notarius</h3>
      <p>Glabro quidam sub vultu latens, odorandi vias periculorum occultas perquam sagax. is in Brittanniam missus ut militares quosdam perduceret ausos conspirasse Magnentio. Hac ita persuasione reducti intra moenia bellatores obseratis undique portarum aditibus.</p>
      <button class="see-more">En savoir plus</button>
    </div>
    <div class="column">
      <h3>Inter quos eminebat notarius</h3>
      <p>Glabro quidam sub vultu latens, odorandi vias periculorum occultas perquam sagax. is in Brittanniam missus ut militares quosdam perduceret ausos conspirasse Magnentio. Hac ita persuasione reducti intra moenia bellatores obseratis undique portarum aditibus.</p>
      <button class="see-more">En savoir plus</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "cardsSection"
}
</script>

<style scoped>
.row{
  display:flex;
}
.column{
  display:flex;
  flex-direction: column;
  width:50%;
  border:solid 1px black
}
</style>