<template>

  <main class="p-4">
      <!-- Main Section - Content goes here -->
      <section class="container">

        <ul class="cards">
            <li v-for="(card, index) in cards" :key="`card-${index}`">
                <Card :thumb="dcComics.thumb" :series="dcComics.series" />
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
        h2 {
            color: white;
        }

        ul {
            display: flex;
            flex-wrap: wrap;
        }
            li {
                width: calc(100% / 6);
            }


</style>