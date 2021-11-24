<template>

  <main class="p-4">
      <!-- Main Section - Content goes here -->
      <section class="container">
        <h3 class="text-uppercase">Current Series</h3>
        <ul class="cards">
            <li v-for="(card, index) in cards" :key="`card-${index}`">
                <Card :thumb="card.thumb" :series="card.series" />
            </li>
        </ul>

      </section>
  </main>

</template>

<script>
import Card from '@/components/Card.vue';
import dcComics from '@/data/dc-comics.js';

export default {
    name: 'Main',
    components: {
        Card,
    },
    data() {
        return {
            cards: dcComics,
        };
        
    },
};
</script>

<style scoped lang="scss">
    main {
        background-color: #1C1C1C;
    }
        h3 {
            color: white;
            background-color: #0282F9;
            max-width: 15%;
            text-align: center;
        }

        ul {
            display: flex;
            flex-wrap: wrap;
        }
            li {
                width: calc(100% / 6);
            }


</style>