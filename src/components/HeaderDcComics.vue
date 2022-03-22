<template>
  <header>
      <div class="logo">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="Logo DC Comics">
          </a>
      </div>
      <nav class="navbar">
          <ul>
            <li v-for="(link, index) in links" :key="index"><a href="link.href">{{ link.text }}</a></li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderDcComics',
  data () {
    return {
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
  }
}
</script>

<style scoper lang="scss">
header {
    display: flex;
    justify-content: space-between;
    .logo {
        vertical-align: middle;
    }
}

li {
    display: inline-block;
    padding: 1rem;
    text-transform: uppercase;
    a {
        display: inline-block;
        text-decoration: none;
        color: black;
    }
}
</style>
