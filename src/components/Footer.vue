<template>
  <footer>
      <section class="container d-flex">
          <!-- Left Top Footer -->
         <div class="left-footer w-50 d-flex py-3">
              <nav class="footer-link-column pe-2">
                <h4 class="pb-2">DC COMICS</h4>
                  <ul>
                      <li class="list-unstyled pb-2" v-for="(link, index) in dcComicsLink" :key="`link-${index}`">
                          <a class="no-decoration" href="/">{{link.text}}</a>
                      </li>
                  </ul>
                  <h4 class="pb-2">SHOP</h4>
                  <ul>
                      <li class="list-unstyled pb-2" v-for="(link, index) in shopLink" :key="`link-${index}`">
                          <a class="no-decoration" href="/">{{link.text}}</a>
                      </li>
                  </ul>
              </nav>
              <nav class="footer-link-column pe-2">
                <h4 class="pb-2">DC</h4>
                  <ul>
                      <li class="list-unstyled pb-2" v-for="(link, index) in dcLink" :key="`link-${index}`">
                          <a class="no-decoration" href="/">{{link.text}}</a>
                      </li>
                  </ul>
              </nav>
              <nav class="footer-link-column">
                <h4 class="pb-2">SITES</h4>
                  <ul>
                      <li class="list-unstyled pb-2" v-for="(link, index) in sitesLink" :key="`link-${index}`">
                          <a class="no-decoration" href="/">{{link.text}}</a>
                      </li>
                  </ul>
              </nav>
         </div>
         <!-- Right Top Footer -->
         <div class="right-footer w-50">
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
            ],
            shopLink: [
                {
                    text: 'Shop DC',
                    url: '/',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '/',
                },
            ],
            dcLink: [
                {
                    text: 'Terms of Use',
                    link: '/',
                },
                {
                    text: 'Privacy Policy (new)',
                    link: '/',
                },
                {
                    text: 'Ad Choices',
                    link: '/',
                },
                {
                    text: 'Advertising',
                    link: '/',
                },
                {
                    text: 'Jobs',
                    link: '/',
                },
                {
                    text: 'Subscription',
                    link: '/',
                },
                {
                    text: 'Talent Workshop',
                    link: '/',
                },
                {
                    text: 'CPSC Certificates',
                    link: '/',
                },
                {
                    text: 'Ratings',
                    link: '/',
                },
                {
                    text: 'Shop Help',
                    link: '/',
                },
                {
                    text: 'Contact Us',
                    link: '/',
                },
            ],
            sitesLink: [
                {
                    text:'DC',
                    url: '/',
                },
                {
                    text:'Mad Magazine',
                    url: '/',
                },
                {
                    text:'DC Kids',
                    url: '/',
                },
                {
                    text:'DC Universe',
                    url: '/',
                },
                {
                    text:'DC Power Visa',
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
        a {
            color: grey;
            font-size: 12px;
        }

        h4 {
            color: white;
            font-weight: 600;
        }

    .right-footer {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position-y: center;
    }
</style>