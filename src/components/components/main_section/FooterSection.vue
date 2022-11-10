<template>
    <section class="footer-section debug d-flex">
        <div class="left-footer-side h-100">
            <div class="container-list">
                <h2 class="text-uppercase">dc comics</h2>
            </div>

            <div class="container-list">
                <h2 class="text-uppercase">shop</h2>
            </div>

            <div class="container-list">
                <h2 class="text-uppercase">dc</h2>
            </div>

            <div class="container-list">
                <h2 class="text-uppercase">sites</h2>
            </div>
        </div>
        <div class="right-footer-side h-100">
        
        </div>

    </section>
</template>

<script>
    export default {
        data(){
            return{
                DcComics: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News',
                ],

                Shop: [
                    'Shop Dc',
                    'Shop Dc Collectibles'
                ],

                DCList: [
                    'Terms Of Use'',
                    'Privacy policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us'
                ],

                SitesList:[
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa',
                ]
            }
        }
        
    }
</script>

<style lang="scss">
    @use '../../../assets/styles/general.scss' as *;

    .footer-section{
        background-image: url(/public/img/footer-bg.jpg);
        height: calc(100vh - 500px);
    }

    .left-footer-side{
        width: calc(100% / 2);
        border: 1px solid red;

    }

    .right-footer-side{
        background-image: url(/public/img/dc-logo-bg.png);
        background-position: center;
        background-repeat: no-repeat;
        z-index: 500;
        color: $hero-img;
        width: calc(100% / 2);
        border: 1px solid yellow;
    }

    h2{
        color: white;
    }

</style>