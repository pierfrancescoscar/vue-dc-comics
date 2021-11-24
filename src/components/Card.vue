<template>
  <div class="card">
      <img class="pb-2 pe-1 square" :src="thumb" :alt="series">
      <h4 class="text-uppercase pb-2">{{ series }}</h4>
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