<template>
  <main>
      <section class="content">
        <div class="container">
          <h3>--&gt; Content goes here &lt;-- </h3>
        </div>
      </section>

      <section class="buy-links">
        <ul class="container">
          <li v-for="(link, index) in buyLinks" :key="index">
            <img :src="'../assets/img/' + link.img" :alt="link.text">
            <span>{{ link.text }}</span>
          </li>
        </ul>
      </section>
  </main>
</template>

<script>
export default {
  name: 'MainDcComics',
  data () {
    return {
      buyLinks: [
        {
          img: 'buy-comics-digital-comics.png',
          text: 'Digital Comics'
        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'DC Merchandise'
        },
        {
          img: 'buy-comics-subscriptions.png',
          text: 'Subscription'
        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'Comic Shop Locator'
        },
        {
          img: 'buy-dc-power-visa.png',
          text: 'DC Power Visa'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/partials/reset.scss";
@import "../assets/scss/partials/variables";
@import "../assets/scss/partials/general";

    main {
        color: white;
        .content {
            padding: 2rem 0;
            background-color: black;
        }
        .buy-links {
            padding: 2rem 0;
            background-color: $blue-dc-color;
            .container {
                display: flex;
                justify-content: space-around;
            }
        }
    }
</style>
