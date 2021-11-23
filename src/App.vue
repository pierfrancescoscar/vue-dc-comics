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
@import '@/styles/utilities.scss';

.active {
  border-bottom: 5px solid #0C7CEC;
}
</style>
