<template>
                <li class="container-img-movie">
                    <img :src="movie.thumb" :alt="movie.series">
                    <h4>{{movie.series}}</h4>
                </li>

</template>

<script>

    export default {

        props: [
            'movie'
        ],
        
    }
</script>

<style lang="scss" scoped>
    @use '../../../assets/styles/general.scss' as *;

    .container-img-movie img{
        height: 250px;     
        max-width: auto;
       
    }

    h4{

        word-wrap: break-word;
    }

</style>