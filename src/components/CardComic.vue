<template>
  <div class="comic-card">
    <img :src="cardImage" :alt="cardTitle">
    <span>{{ cardTitle.toUpperCase() }}</span>
  </div>
</template>

<script>
export default {
  name: 'CardComic',
  props: {
    cardImage: String,
    cardTitle: String
  }
}
</script>

<style lang="scss">
@import "../assets/scss/partials/reset.scss";
@import "../assets/scss/partials/variables";
@import "../assets/scss/partials/general";

.comic-card {
        flex-basis: calc((100% / 6) - 2rem);
        img {
          width: 100%;
          height: 155px;
          object-fit: cover;
          object-position: top;
        }
}

</style>
