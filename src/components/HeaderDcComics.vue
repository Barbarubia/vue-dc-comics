<template>
  <header>
      <div class="logo">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="Logo DC Comics">
          </a>
      </div>
      <nav class="navbar">
          <ul>
            <li @click="setActiveIndex(index)" v-for="(link, index) in links" :key="index" :class="{active: index == activeIndex}"><a href="link.href">{{ link.text }}</a></li>
          </ul>
      </nav>
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
header {
    height: 5rem;
    display: flex;
    justify-content: space-between;
    .logo {
        img {
            height: 100%;
        }
    }
}

li {
    height: 5rem;
    display: inline-block;
    padding: 0 1rem;
    text-transform: uppercase;
    &.active {
        border-bottom: 2px solid green;
    }
    a {
        display: inline-block;
        text-decoration: none;
        color: black;
        font-weight: 600;
    }
}
</style>
