<template>
  <header class="container">
      <div class="logo">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="Logo DC Comics">
          </a>
      </div>
      <ul class="navbar">
          <li @click="setActiveIndex(index)" v-for="(link, index) in links" :key="index" :class="{active: index == activeIndex}"><a :href="link.href" :class="{active: index == activeIndex}">{{ link.text }}</a></li>
      </ul>
  </header>
</template>

<script>
export default {
  name: 'HeaderDcComics',
  data () {
    return {
      activeIndex: 1,
      links: [
        {
          href: '#',
          text: 'Characters'
        },
        {
          href: '#',
          text: 'Comics'
        },
        {
          href: '#',
          text: 'Movies'
        },
        {
          href: '#',
          text: 'TV'
        },
        {
          href: '#',
          text: 'Games'
        },
        {
          href: '#',
          text: 'Collectibles'
        },
        {
          href: '#',
          text: 'Videos'
        },
        {
          href: '#',
          text: 'Fans'
        },
        {
          href: '#',
          text: 'News'
        },
        {
          href: '#',
          text: 'Shop'
        }
      ]
    }
  },
  methods: {
    setActiveIndex (index) {
      this.activeIndex = index
    }
  }
}
</script>

<style scoper lang="scss">
@import "../assets/scss/partials/reset.scss";
@import "../assets/scss/partials/variables";
@import "../assets/scss/partials/general";

header {
    padding: .5rem 0;
    display: flex;
    justify-content: space-between;
    .logo {
        height: 5rem;
        img {
            height: 100%;
            vertical-align: middle;
        }
    }
}

.navbar {
    height: 5rem;
    li {
    height: 5rem;
    display: inline-block;
    margin: 0 1rem 0 1rem;
    line-height: 5rem;
    text-transform: uppercase;
        a {
            display: inline-block;
            line-height: 5rem;
            vertical-align: middle;
            text-decoration: none;
            color: black;
            font-weight: 600;
            &.active {
                border-bottom: 2px solid $blue-dc-color;
                color: $blue-dc-color;
                }
        }
    }
}
</style>
