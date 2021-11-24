<template>
  <div class="card">
      <img :src="thumb" :alt="series">
      <h4>{{ series }}</h4>
  </div>
</template>

<script>

export default {
    name: 'Card',
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>

<style scoped lang="scss">
.card {
    background: red;
}

</style>