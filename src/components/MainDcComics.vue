<template>
  <main>
    <section class="content">
      <div class="container">
        <h2>--&gt; Content goes here &lt;-- </h2>
      </div>
    </section>

    <section class="buy-links">
      <ul class="container">
        <li v-for="(link, index) in buyLinks" :key="index">
          <a :href="link.href">
            <img :src="require('../assets/img/' + link.img)" :alt="link.text">
            <span>{{ link.text }}</span>
          </a>
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
          href: '#',
          img: 'buy-comics-digital-comics.png',
          text: 'Digital Comics'
        },
        {
          href: '#',
          img: 'buy-comics-merchandise.png',
          text: 'DC Merchandise'
        },
        {
          href: '#',
          img: 'buy-comics-subscriptions.png',
          text: 'Subscription'
        },
        {
          href: '#',
          img: 'buy-comics-shop-locator.png',
          text: 'Comic Shop Locator'
        },
        {
          href: '#',
          img: 'buy-dc-power-visa.svg',
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
        padding: 3rem 0;
        background-color: black;
    }
    .buy-links {
        padding: 3rem 0;
        background-color: $blue-dc-color;
        .container {
            display: flex;
            justify-content: space-around;
            align-items: center;
            list-style: none;
            li {
              text-transform: uppercase;
            }
            img {
              height: 3rem;
              vertical-align: middle;
              margin-right: .5rem;
            }
            a {
              text-decoration: none;
              color: white;
            }
        }
    }
}
</style>
