<template>
    <footer class="debug">
        <div class="container myWrapper debug h-100 d-flex space-between align-items-center">
                 <!-- FOOTER LEFT SIDE -->

            <div class="left-side">
                    <div class="sign-up text-uppercase fs-m">sign-up</div>
            </div>

                <!-- FOOTER RIGHT SIDE -->

            <div class="right-side d-flex align-items-center">
                <div class="follow-footer text-uppercase fs-m">follow us</div>

                    <!-- CONTAINER ICON SOCIAL FOOTER -->

                <div class="container-icon d-flex align-items-center">
                    <div class="circle-icon" v-for="(social, index) in iconList" :key="index">
                        <img :src="social" alt="social icon">
                    </div>
                </div>
            </div>
        </div>

    </footer>
</template>

<script>
    export default {
        data() {
            return {
                iconList: [
                   '/public/img/footer-facebook.png',
                   '/public/img/footer-twitter.png',
                   '/public/img/footer-youtube.png',
                   '/public/img/footer-pinterest.png',
                   '/public/img/footer-periscope.png',
                ]
            }
        }
        
    }
</script>

<style lang="scss">
@use '../../assets/styles/general.scss' as *;

    footer{
        height: 100px;
        color: black;
        background-color: $bg-icon-footer;
    }

    .left-side{
        color: white;

        .sign-up{
            border: 1px solid $white;
            width: max-content;
            padding: 5px;
        }
        .sign-up:hover{
            border: 1px solid $hero-img;
            cursor: pointer;
        }
        
    }
    .follow-footer{
        color: $hero-img;
        font-weight: bold;
    }

    .circle-icon{
       

        img{
            color: $bg-icon-footer;
            
        }
    }
</style>