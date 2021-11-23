<template>
<div class="bottom-footer p-3">
  <section class="container d-flex">
      <div class="left-bottom-footer w-50">
          <button class="text-uppercase p-2">Sign-up now!</button>
      </div>

      <div class="right-bottom-footer w-50 d-flex">
          <h4 class="text-uppercase">Follow us</h4>
          
      </div>
  </section>
</div>
</template>

<script>
export default {
    name: 'BottomFooter'
}
</script>

<style scoped lang="scss">
    .bottom-footer {
        background-color: #303030;
    }
        button {
            background: transparent;
            color: white;
            border: 1px solid #0282F9;
        }
</style>