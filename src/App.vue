<template>
  <div id="app">
    <HeaderDcComics />
    <MainDcComics />
  </div>
</template>

<script>
import HeaderDcComics from './components/HeaderDcComics.vue'
import MainDcComics from './components/MainDcComics.vue'

export default {
  name: 'App',
  components: {
    HeaderDcComics,
    MainDcComics
  }
}
</script>

<style scoped lang="scss">
@import "./assets/scss/style.scss";
</style>
