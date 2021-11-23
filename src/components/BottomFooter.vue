<template>
<div class="bottom-footer p-3">
  <section class="container d-flex align-items-center">
      <div class="left-bottom-footer w-50">
          <button class="text-uppercase p-2">Sign-up now!</button>
      </div>

      <div class="right-bottom-footer w-50 d-flex">
          <h4 class="pe-2 text-uppercase">Follow us</h4>
          <div class="social-links">
              <img class="pe-2" src="../assets/img/footer-facebook.png" alt="">
              <img class="pe-2" src="../assets/img/footer-periscope.png" alt="">
              <img class="pe-2" src="../assets/img/footer-pinterest.png" alt="">
              <img class="pe-2" src="../assets/img/footer-twitter.png" alt="">
              <img class="pe-2" src="../assets/img/footer-youtube.png" alt="">
          </div>
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
        h4 {
            color: #0282F9;
        }
        button {
            cursor: pointer;
            background: transparent;
            color: white;
            border: 1px solid #0282F9;
        }
</style>