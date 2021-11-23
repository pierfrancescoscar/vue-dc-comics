<template>
  <footer class="p-4">
      <section class="container">
         <div class="left-footer w-50">
              <nav>
                  <ul>
                      <li class="list-unstyled" v-for="(link, index) in dcComicsLink" :key="`link-${index}`">
                          <a href="/">{{link.text}}</a>
                      </li>
                  </ul>
              </nav>
         </div>
      </section>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            dcComicsLink: [
                {
                    text: 'Characters',
                    url: '/',
                },
                {
                    text: 'Comics',
                    url: '/',
                    
                },
                {
                    text: 'Movies',
                    url: '/',
                   
                },
                {
                    text: 'TV',
                    url: '/',
                    
                },
                {
                    text: 'Games',
                    url: '/',
                    
                },
                {
                    text: 'Videos',
                    url: '/',
                    
                },
                {
                    text: 'News',
                    url: '/',
                    
                },
            ]
        }
    }

}
</script>

<style scoped lang="scss">
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        background-position: center;
    }
</style>