<template>
    <section class="footer-section debug d-flex">
        <div class="left-footer-side h-100"></div>
        <div class="right-footer-side h-100">
        
        </div>

    </section>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss">
    @use '../../../assets/styles/general.scss' as *;

    .footer-section{
        background-image: url(../../../assets/img/footer-bg.jpg);
        height: calc(100vh - 500px);
    }

    .left-footer-side{
        width: calc(100% / 2);
        border: 1px solid red;

    }

    .right-footer-side{
        background-image: url(../../../assets/img/dc-logo-bg.png);
        background-position: center;
        background-repeat: no-repeat;
        z-index: 500;
        color: $hero-img;
        width: calc(100% / 2);
        border: 1px solid yellow;


    }

</style>