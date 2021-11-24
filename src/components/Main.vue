<template>

  <main class="p-4">
      <!-- Main Section - Content goes here -->
      <section class="container">
        <span class="text-uppercase p-2">Current Series</span>
        <ul class="cards">
            <li class="list-unstyled pb-2" v-for="(card, index) in cards" :key="`card-${index}`">
                <Card :thumb="card.thumb" :series="card.series" />
            </li>
        </ul>
        <div class="load-more d-flex justify-content-center">
            <button class="text-uppercase p-2">Load more</button>
        </div>
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
        span {
            color: white;
            font-weight: 600;
            background: #0282F9;
            position: absolute;
            top: 60%;
        }

        ul {
            display: flex;
            flex-wrap: wrap;
        }
            li {
                width: calc(100% / 6);
            }

        button {
            border: none;
            background: #0282F9;
            color: white;
            font-weight: 600;
            
        }


</style>