<template>
    <footer class="debug">
        <div class="container myWrapper debug h-100 d-flex space-between align-items-center">
                 <!-- FOOTER LEFT SIDE -->

            <div class="left-side">
                    <div class="sign-up text-uppercase fs-m">sign-up</div>
            </div>

                <!-- FOOTER RIGHT SIDE -->

            <div class="right-side d-flex align-items-center space-between">
                <div class="follow-footer text-uppercase fs-m">follow us</div>

                    <!-- CONTAINER ICON SOCIAL FOOTER -->

                <div class="container-icon d-flex align-items-center space-between">
                    <div class="circle-icon" v-for="(icon, index) in iconList" :key="index">{{icon}}</div>
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
                   '<i class="fa-brands fa-facebook"></i>',
                   '<i class="fa-brands fa-twitter"></i>',
                   '<i class="fa-brands fa-youtube"></i>',
                   '<i class="fa-brands fa-pinterest"></i>',
                   '<i class="fa-solid fa-location-dot"></i>',
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
</style>