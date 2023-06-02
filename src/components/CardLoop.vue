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
          imageSrc: 'image1.jpg',
          title: 'Augustum actus eius exaggerando',
          description: 'Nam utilitates quidem etiam ab iis percipiuntur antiquior et pulchrior.',
          date: '2022-01-01',
        },
        {
          imageSrc: 'image2.jpg',
          title: 'Thalassius vero ea tempestate',
          description: 'Recipiendisque meritis quod quisque minus ut dandis recipiendisque.',
          date: '2021-12-17',
        },
        {
          imageSrc: 'image2.jpg',
          title: 'Vexillum altius erigens posticas',
          description: 'Utrum propter imbecillitatem atque inopiam posticas in regiam.',
          date: '2021-11-05',
        },
        {
          imageSrc: 'image2.jpg',
          title: 'Opposita instar rapidi fluminis',
          description: 'Saepissime igitur mihi de amicitia cogitanti maxime fingerent quaedam.',
          date: '2021-06-24',
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-loop {
}
</style>
