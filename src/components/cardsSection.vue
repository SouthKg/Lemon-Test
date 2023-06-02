<template>
  <div class="row">
    <div class="column first">
      <h3>Inter quos eminebat notarius</h3>
      <p>Glabro quidam sub vultu latens, odorandi vias periculorum occultas perquam sagax. is in Brittanniam missus ut militares quosdam perduceret ausos conspirasse Magnentio. Hac ita persuasione reducti intra moenia bellatores obseratis undique portarum aditibus.</p>
      <button class="see-more">En savoir plus</button>
    </div>
    <div class="column second">
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
  margin-top:50px;
  margin-bottom:50px;
  margin-left:17%;
  margin-right:17%;
}
.column{
  display:flex;
  flex-direction: column;
  width:50%;
  border:solid 1px black;
  padding:45px;
}
h3{
  margin-top:0px;
  text-align: left;
}
p{
  text-align: left;
  margin-bottom:20px;
}
.first{
  background:#212529;
  color:white;
  margin-right:10px;
}
button{
  cursor: pointer;
  width:130px;
  padding-top:10px;
  padding-bottom:10px;
  font-size:15px;
  background:none;
}
.first button{
  border:white solid 1px;
  color:white;
  transition:0.6s;
}
.first button:hover{
  color:#212529;
  background:white;
  transition:0.6s;
}
.second{
  background:##F8F9FA;
  margin-left:10px;
  border-color:#DEE2E6;
}
.second button{
  border:#6C757D solid 1px;
  color:#6C757D;
  transition:0.6s;
}
.second button:hover{
  color:white;
  background:#6C757D;
  transition:0.6s;
}
@media screen and (max-width:1024px){
  .row{
    flex-direction: column;
    margin-left:15px;
    margin-right:15px;
  }
  .column{
    width:72%;
    margin-right:0px;
    margin-left:0px;
    margin-bottom:20px;
  }
}
</style>