<template>
  <div id="app">
    <HeaderDcComics />
    <MainDcComics />
    <FooterDcComics />
  </div>
</template>

<script>
import HeaderDcComics from './components/HeaderDcComics.vue'
import MainDcComics from './components/MainDcComics.vue'
import FooterDcComics from './components/FooterDcComics.vue'

export default {
  name: 'App',
  components: {
    HeaderDcComics,
    MainDcComics,
    FooterDcComics
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
