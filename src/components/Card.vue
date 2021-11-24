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

    h4 {
        color: white;
        font-size: 14px;
        font-weight: 400;
    }
}
</style>