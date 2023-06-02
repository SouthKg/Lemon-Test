<template>
  <div class="card-actu">
    <img :src="imageSrc" alt="Image">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
    <div class="row">
      <div class="column">
        <p>{{ date }}</p>
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
  /* Styles for cardActu component */
}

.row {
  display: flex;
}

.column {
  flex: 1;
}
</style>
