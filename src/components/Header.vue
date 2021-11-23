<template>
  <header class="container">
      <!-- Left - Logo -->
      <a href="/">
        <img src="../assets/img/dc-logo.png" alt="dc-logo">
      </a>
      <!-- Right - Menu -->
      <nav>
          <ul>
              <li v-for="(link, index) in menuLink" :key="`link-${index}`">
                  <a :class="{active: link.current}" :href="link.url">
                      {{link.text}}
                    </a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            menuLink: [
                {
                    text: 'CHARACTERS',
                    url: '/',
                    current: true,
                },
                {
                    text: 'COMICS',
                    url: '/',
                    current: false,
                },
                {
                    text: 'MOVIES',
                    url: '/',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '/',
                    current: false,
                },
                {
                    text: 'GAMES',
                    url: '/',
                    current: false,
                },
                {
                    text: 'COLLECTIBLES',
                    url: '/',
                    current: false,
                },
                {
                    text: 'VIDEOS',
                    url: '/',
                    current: false,
                },
                {
                    text: 'FANS',
                    url: '/',
                    current: false,
                },
                {
                    text: 'NEWS',
                    url: '/',
                    current: false,
                },
                {
                    text: 'SHOP',
                    url: '/',
                    current: false,
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

</style>