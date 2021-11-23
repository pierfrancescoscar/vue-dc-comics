<template>
  <header class="container p-2 d-flex align-items-center">
      <!-- Left - Logo -->
    <div class="w-50">
      <a href="/">
        <img class="pe-2" src="../assets/img/dc-logo.png" alt="dc-logo">
      </a>
    </div>
      <!-- Right - Menu -->
    <div class="w-50">
      <nav>
          <ul>
              <li v-for="(link, index) in menuLink" :key="`link-${index}`">
                  <a class="pe-1" :class="{active: link.current}" :href="link.url">
                      {{link.text}}
                    </a>
              </li>
          </ul>
      </nav>
    </div>
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
    ul {
        display: flex;
        list-style: none;
    }
        a {
            display: inline-block;
            text-decoration: none;
            font-size: 14px;
            color: black;
            font-weight: 600;
            &:hover {
            color: #0C7CEC;
        }
        }
        


</style>