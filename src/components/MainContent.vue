<template>
  <section class="content">
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

main {
  color: white;
  .content {
      padding: 3rem 0;
      background-color: black;
  }
}
</style>
