<template>
    <main class="debug">
        <div class="container myWrapper debug">

              <section><HeaderSection/></section>

              <section><MainSection/></section>

              <section><FooterSection/></section>
        </div>

    </main>
</template>

<script>
import FooterSection from './main_section/FooterSection.vue';
import HeaderSection from './main_section/HeaderSection.vue';
import MainSection from './main_section/MainSection.vue';

    export default {
    components: { HeaderSection, MainSection, FooterSection }
}
</script>

<style lang="scss">
    @use '../../assets/styles/general.scss' as *;

    .container{
        height: calc(100vh - 200px);
    }

</style>