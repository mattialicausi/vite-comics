<template>
    <section class="main-section">
        <div class="myWrapper text-uppercase h-100">
            <ul class="d-flex align-items-center space-around w-100 h-100">
                <li class="d-flex align-items-center " v-for="(card, index) in mainCard" :key="index">
                    <img :src="card.image" :alt="'image of ' + card.text">
                    <h3>{{card.text}}</h3>
                </li>
            </ul>
        </div>

        

    </section>
</template>

<script>
    export default {
        data(){
            return{
                mainCard: [
                    {
                        image: '/public/img/buy-comics-digital-comics.png',
                        text: 'digital comics'
                    },
                    {
                        image: '/public/img/buy-comics-merchandise.png',
                        text: 'dc merchandise'
                    },
                    {
                        image: '/public/img/buy-comics-subscriptions.png',
                        text: 'subscription'
                    },
                    {
                        image: '/public/img/buy-comics-shop-locator.png',
                        text: 'comic shop location'
                    },
                    {
                        image: '/public/img/buy-dc-power-visa.svg',
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
        height: 80px;
        
    }

    h3 {
        padding-left: 5px;
        font-size: 13px;
    }

</style>