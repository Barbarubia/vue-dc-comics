<template>
  <div>
    <img :src="cardImage" :alt="cardTitle">
    <h2>{{ cardTitle }}</h2>
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

<style>

</style>
