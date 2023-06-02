<template>
  <div class="card-actu">
    <img :src="imageSrc" alt="Image">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
    <div class="row">
      <div class="column">
        <p><img class="calendar-img" src="../assets/CalendarEvent.png" alt="Calendar"> {{
            date }}</p>
      </div>
      <div class="column">
        <button>En savoir plus</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageSrc: String,
    title: String,
    description: String,
    date: String,
  },
};
</script>

<style scoped>
.card-actu {
  display:flex;
  width:15%;
  flex-direction: column;
  margin-left:15px;
  margin-right:15px;
  border:solid 1px #00000020;

}

.row {
  display: flex;
  background:#00000008;
  border:solid 1px #00000020;
}

.column {
  flex: 1;
}

img{
  height:170px;
  width:100%;
  object-fit: cover;
}

h2, p{
  text-align: left;
  margin-left:10px;
  margin-right:10px;
}
img.calendar-img{
  height:14px;
  width:14px;
}

.row button{
  background:#6C757D;
  border:none;
  padding:10px;
  cursor: pointer;
  color:white;
  font-size:16px;
  margin-top:5px;
}
</style>
