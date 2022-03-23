<template>
  <section class="content">
    <div class="jumbo"></div>

    <div class="container">
      <h2>--&gt; Content goes here &lt;-- </h2>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MainContent'
}
</script>

<style lang="scss">
@import "../assets/scss/partials/reset.scss";
@import "../assets/scss/partials/variables";
@import "../assets/scss/partials/general";

.content {
        background-color: $main-dark-bg;
        color: white;
      .jumbo {
        height: 25rem;
        background-image: url(../assets/img/jumbotron.jpg);
      }
      .container {
        padding: 3rem 0;
      }
}
</style>
