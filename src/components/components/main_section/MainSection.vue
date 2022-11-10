<template>
    <section class="main-section debug text-uppercase d-flex space-between align-items-center">

        <ul class="d-flex align-items-center space-between">
            <li class="d-flex" v-for="(card, index) in mainCard" :key="index">
                <img :src="'../../../' + card.image" :alt="'image of ' + card.text">
                <h3 class="fs-s">{{card.text}}</h3>
            </li>
            <img src="../../../assets/img/buy-comics-digital-comics.png" alt="">
        </ul>

    </section>
</template>

<script>
    export default {
        data(){
            return{
                mainCard: [
                    {
                        image: 'assets/img/buy-comics-digital-comics.png',
                        text: 'digital comics'
                    },
                    {
                        image: 'assets/img/buy-comics-merchandise.png',
                        text: 'dc merchandise'
                    },
                    {
                        image: 'assets/img/buy-comics-subscriptions.png',
                        text: 'subscription'
                    },
                    {
                        image: 'assets/img/buy-comics-shop-locator.png',
                        text: 'comic shop location'
                    },
                    {
                        image: 'assets/img/buy-dc-power-visa.svg',
                        text: 'dc power visa'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss">
    @use '../../../assets/styles/general.scss' as *;

    .main-section{
        height: 150px;
        background-color: $hero-img;
        color: white;

    }

    li img{
        height: 90px;
        width: auto;
    }

</style>