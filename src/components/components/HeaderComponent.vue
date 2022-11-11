<template>
    <header>

            <!-- CONTENITORE IMG HEADER -->
        <div class="top-header d-flex space-between myWrapper">
            <div class="container-logo-header d-flex align-items-center pb-2">
                <img src="/public/img/dc-logo.png" alt="Logo DC">
            </div>
        
            <!-- CONTENITORE NAV BAR HEADER -->

            <div class="container-nav-bar">
                <div class="nav-bar h-100">
                    <ul class="d-flex align-items-center ul-header h-100">
                        <li class="text-uppercase fs-s d-flex align-items-center" v-for="(items, index) in childNav" :key="index">{{items}}</li>
                    </ul>
                </div>
            </div>  
        </div>


        <!-- CONTAINER JUMBO -->

    <div class="jumbo">
        <HeaderJumbo/>
    </div>

    </header>

</template>

<script>
import HeaderJumbo from './header_section/HeaderJumbo.vue';

    export default {
    data() {
        return {
            childNav: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop",
            ]
        };
    },
    components: { HeaderJumbo }
}
</script>

<style lang="scss">
    @use '../../assets/styles/general.scss' as *;

    .top-header{
        height: 10vh;
    }

    .jumbo{
        height: 30vh;
        background-image: url(../../../public/img/jumbotron.jpg);
        background-size: cover;
    }

    header {
        width: 100%;
    }

    .container-logo-header{
        height: 100px;
        width: 100px;

        img{
            width: 80px;
            height: 80px;
        }
    }

    .ul-header{
        list-style: none;

        li{
            padding: 10px;
            height: 100%;
        }

        li:hover{
            border-bottom: 1px solid $hero-img;
            color: $hero-img;
            cursor: pointer;

        }
    }


</style>