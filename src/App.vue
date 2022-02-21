<template>
  <div id="app" class="container">

    <HeaderComponent></HeaderComponent>

    <MainTop></MainTop>

    <MainBottom></MainBottom>

    <FooterTop></FooterTop>

    <FooterBottom></FooterBottom>
    
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainTop from './components/MainTop.vue'
import MainBottom from './components/MainBottom.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainTop,
    MainBottom,
    FooterTop,
    FooterBottom
  }
}
</script>

<style lang="scss">

  @import "./assets/style/general.scss";

</style>
