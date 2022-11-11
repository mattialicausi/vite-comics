<template>
    <main>
        <div class="container">

              <section class="header-section-main h-100">

                <div>
                    <div class="container-content myWrapper debug h-100 text-uppercase">
                        <ul class="container-movie d-flex wrap">
                            <HeaderSection v-for="(item, index) in listMovie" :key="index" :movie="item" />
                        </ul>
                       
                    </div>
                </div>
             
              </section>

              <section><MainSection/></section>

              <section><FooterSection/></section>
        </div>

    </main>
</template>

<script>
import {movieList} from '../../data/data_list';

import FooterSection from './main_section/FooterSection.vue';
import HeaderSection from './main_section/HeaderSection.vue';
import MainSection from './main_section/MainSection.vue';

    export default {
    components: { HeaderSection, MainSection, FooterSection },

    data(){
        return {
            listMovie : movieList,
        }
    }
}
</script>

<style lang="scss">
    @use '../../assets/styles/general.scss' as *;

    .header-section-main{
        height: calc(100vh - 40vh);
        background-color: $contents;
        width: 100%;
        color: white;
    }

    .container-content{
        width: calc(100% / 6);
        margin: 0 auto;
        

    }

    .container-movie{
        //width: calc(100% / 6);
        list-style: none;
    }

</style>