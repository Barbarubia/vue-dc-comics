<template>
  <div id="app">
    <HeaderDcComics />
  </div>
</template>

<script>
import HeaderDcComics from './components/HeaderDcComics.vue'

export default {
  name: 'App',
  components: {
    HeaderDcComics
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
