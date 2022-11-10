<template>
  <header>
    <HeaderComponent />
  </header>

  <main>
    <MainComponent />
  </main>

  <footer>
    <FooterComponent />
  </footer>
 
</template>

<script>
import HeaderComponent from './components/components/HeaderComponent.vue';
import MainComponent from './components/components/MainComponent.vue';
import FooterComponent from './components/components/FooterComponent.vue';


  export default {
    components: { HeaderComponent, MainComponent, FooterComponent}
}
</script>

<style lang="scss" scoped>
@use './assets/styles/general.scss' as *;
</style>
