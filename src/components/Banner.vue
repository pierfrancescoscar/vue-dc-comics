<template>
    <div class="blue-banner p-3">
            <section class="container">
                <ul>
                    <li class="list-unstyled" v-for="(item, index) in shopList" :key="`shopitem-${index}`">
                        <img :src="item.img" :alt="item.name">
                        <a href="/">
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
                    img: require('@/assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics',

                },
                {
                    img: require('@/assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics',

                },
                {
                    img: require('@/assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics',

                },
                {
                    img: require('@/assets/img/buy-comics-digital-comics.png'),
                    name: 'Digital Comics',

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
    }

</style>