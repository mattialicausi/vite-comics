<template>
    <header class="d-flex space-between">
        <div class="container-logo-header d-flex align-items-center">
            <img src="./../../assets/img/dc-logo.png" alt="Logo DC">
        </div>

        <div class="container-nav-bar">
            <div class="nav-bar h-100">
                <ul class="d-flex align-items-center">
                    <li class="text-uppercase fs-s d-flex align-items-center" v-for="(items, index) in childNav" :key="index">{{items}}</li>
                </ul>
            </div>
        
        </div>
    </header>
</template>

<script>
    export default {
        data(){
            return {
                childNav: [
                    'characters',
                    'comics',
                    'movies',
                    'tv',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop',

                ]
            }
        }
        
    }
</script>

<style lang="scss">
    @use '../../assets/styles/general.scss' as *;

    header {
        height: 100px;
        width: 100%;
        border: 1px solid red;
    }

    .container-logo-header{
        height: 100px;
        width: 100px;

        img{
            width: 80px;
            height: 80px;
        }
    }

    ul{
        list-style: none;
        height: 100%;

        li{
            padding: 10px;
            height: 100%;
        }

        li:hover{
            border-bottom: 1px solid $hero-img;
        }
    }



</style>