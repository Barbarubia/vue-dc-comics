<template>
  <main>
    <MainContent />
    <MainBlueSection />
  </main>
</template>

<script>
import MainContent from './MainContent.vue'
import MainBlueSection from './MainBlueSection.vue'

export default {
  name: 'MainDcComics',
  components: {
    MainContent,
    MainBlueSection
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/partials/reset.scss";
@import "../assets/scss/partials/variables";
@import "../assets/scss/partials/general";
</style>
