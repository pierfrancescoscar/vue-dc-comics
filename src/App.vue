<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Hero -->
    <Hero />
    <!-- Main -->
    <Main />
    <!-- Footer -->
    <Footer />
    <!-- Bottom Footer -->
    <BottomFooter />
  </div>
</template>

<script>
import Hero from '@/components/Hero.vue';
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';
import BottomFooter from '@/components/BottomFooter.vue';
import Card from '@/components/Card.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    BottomFooter,
    Hero,
    Card,
  }
}
</script>

<style lang="scss">
@import '@/styles/global.scss';
@import '@/styles/utilities.scss';

.active {
  border-bottom: 5px solid #0C7CEC;
}
</style>
