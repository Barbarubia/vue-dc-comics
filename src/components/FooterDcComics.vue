<template>
  <footer>
      <section class="main-footer container">
          <ul class="footer-links-container">
              <li v-for="(element, index) in Categories" :key="index">
                  <h3>{{ element.category }}</h3>
                  <ul>
                      <li v-for="(sublink, subindex) in element.subLinks" :key="subindex"><a href="sublink.href">{{ sublink.name }}</a></li>
                  </ul>
              </li>
          </ul>
      </section>
      <section class="footer-navbar">
          <div class="container">
              <button>Sign un now!</button>
              <div class="social-networks">
                  <h3>Follow us</h3>
                  <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                  <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                  <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                  <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                  <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
              </div>
          </div>
      </section>
  </footer>
</template>

<script>
export default {
  name: 'FooterDcComics',
  data () {
    return {
      Categories: [
        {
          category: 'DC Comics',
          subLinks: [
            {
              href: '#',
              name: 'Characters'
            },
            {
              href: '#',
              name: 'Comics'
            },
            {
              href: '#',
              name: 'Movies'
            },
            {
              href: '#',
              name: 'TV'
            },
            {
              href: '#',
              name: 'Gamess'
            },
            {
              href: '#',
              name: 'Videos'
            },
            {
              href: '#',
              name: 'News'
            }
          ]
        },
        {
          category: 'Shop',
          subLinks: [
            {
              href: '#',
              name: 'Shop DC'
            },
            {
              href: '#',
              name: 'Shop DC Collectibles'
            }
          ]
        },
        {
          category: 'DC',
          subLinks: [
            {
              href: '#',
              name: 'Terms Of Use'
            },
            {
              href: '#',
              name: 'Privacy policy (New)'
            },
            {
              href: '#',
              name: 'Ad Choices'
            },
            {
              href: '#',
              name: 'Advertising'
            },
            {
              href: '#',
              name: 'Jobs'
            },
            {
              href: '#',
              name: 'Subscriptions'
            },
            {
              href: '#',
              name: 'Talent Workshops'
            },
            {
              href: '#',
              name: 'CPSC Certificates'
            },
            {
              href: '#',
              name: 'Ratings'
            },
            {
              href: '#',
              name: 'Shop Help'
            },
            {
              href: '#',
              name: 'Contact Us'
            }
          ]
        },
        {
          category: 'Sites',
          subLinks: [
            {
              href: '#',
              name: 'DC'
            },
            {
              href: '#',
              name: 'MAD Magazine'
            },
            {
              href: '#',
              name: 'DC Kids'
            },
            {
              href: '#',
              name: 'DC Universe'
            },
            {
              href: '#',
              name: 'DC Power Visa'
            }
          ]
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

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    .main-footer {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position-x: right;
        background-position-y: center;
        background-size: 30rem;
        display: flex;
        justify-content: flex-start;
    }
}

ul {
    list-style: none;
    h3 {
        text-transform: uppercase;
        color: white;
        margin-bottom: 1rem;
    }
}

.footer-links-container {
    padding: 2rem 0;
    height: 22rem;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 1rem;
    a {
        text-decoration: none;
        color: #828282;
    }
}

.footer-navbar {
    padding: 2rem 0;
    background-color: #303030;
    background-image: none;
    .container {
        display: flex;
        justify-content: space-between;
        button {
            background: none;
            border: 1px solid $blue-dc-color;
            padding: .5rem;
            text-transform: uppercase;
        }
    }
}
</style>
