<template>
  <h2>Actualités du groupe Veolia</h2>
  <div class="card-loop">
    <CardActu v-for="(card, index) in cards" :key="index" :image-src="card.imageSrc" :title="card.title" :description="card.description" :date="card.date" />
  </div>
</template>

<script>
import CardActu from './CardActu.vue';

export default {
  components: {
    CardActu,
  },
  data() {
    return {
      cards: [
        {
          imageSrc: require('../assets/img-article1.png'),
          title: 'Augustum actus eius exaggerando',
          description: 'Nam utilitates quidem etiam ab iis percipiuntur antiquior et pulchrior.',
          date: '01/01/2022',
        },
        {
          imageSrc: require('../assets/img-article2.png'),
          title: 'Thalassius vero ea tempestate',
          description: 'Recipiendisque meritis quod quisque minus ut dandis recipiendisque.',
          date: '17/12/2021',
        },
        {
          imageSrc: require('../assets/img-article3.png'),
          title: 'Vexillum altius erigens posticas',
          description: 'Utrum propter imbecillitatem atque inopiam posticas in regiam.',
          date: '05/11/2021',
        },
        {
          imageSrc: require('../assets/img-article4.png'),
          title: 'Opposita instar rapidi fluminis',
          description: 'Saepissime igitur mihi de amicitia cogitanti maxime fingerent quaedam.',
          date: '24/04/2021',
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-loop {
  display:flex;
  flex-direction: row;
  justify-content: center;
  margin-bottom: 50px;
}
h2{
  text-align: left;
  margin-left:18%;
}
</style>
