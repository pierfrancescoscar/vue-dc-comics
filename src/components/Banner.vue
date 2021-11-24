<template>
    <div class="blue-banner p-3">
            <section class="container">
                <ul>
                    <li class="list-unstyled" v-for="(item, index) in shopList" :key="`shopitem-${index}`">
                        <img :src="item.img" :alt="item.name">
                        <a class="no-decoration text-uppercase" href="/">
                        {{item.name}}
                        </a>
                    </li>
                </ul>
            </section>
    </div>
</template>

<script>
export default {
    name: 'Banner',
    data () {
        return {
            shopList: [
                {
                    img: require('@/assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics',

                },
                {
                    img: require('@/assets/img/buy-comics-merchandise.png'),
                    name: 'DC Merchandise',

                },
                {
                    img: require('@/assets/img/buy-comics-subscriptions.png'),
                    name: 'Subscription',

                },
                {
                    img: require('@/assets/img/buy-comics-shop-locator.png'),
                    name: 'Comic Shop Locator',

                },
                {
                    img: require('@/assets/img/buy-dc-power-visa.svg'),
                    name: 'DC Power VISA',

                },
                
            ]
        }
    }

}
</script>

<style scoped lang="scss">
.blue-banner {
        background-color: #0C7CEC;
    }
    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        justify-content: space-between;
    }
        a {
            color: white;
            font-weight: 400;
        }

        img {
            width: 50px;
            height: 50px;
            object-fit: contain;
        }
        

</style>