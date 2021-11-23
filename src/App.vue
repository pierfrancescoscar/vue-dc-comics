<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- Main -->

    <!-- Footer -->

  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
@import '@/styles/global.scss';
@import '@/styles/utilities.scss'
</style>
