<template>
  <div id="app">
    <Header />
      <div class="content-wrap">
        <FloatButton v-if="showFlatButton" />
        <Home />
        <Services />
        <Offer />
        <Reviews />
        <Contact />
      </div>
    <Footer/>
    <MobileMenu />
  </div>
</template>

<script>
import Header from './partials/HeaderPartial.vue'
import Footer from './partials/FooterPartial.vue'
import Home from './views/Home'
import Services from './views/Services'
import Offer from './views/Offer'
import Reviews from './views/Reviews';
import Contact from './views/Contact';
import FloatButton from './components/FloatButton';
import MobileMenu from './components/MobileMenu';

export default {
  name: 'app',
  components: {
    Header, Footer, Home, Services, Offer, Reviews, Contact, FloatButton, MobileMenu
  },
  data() {
    return {
      showFlatButton: false,
      lastScrollPosition: 0
    }
  },
  methods: {
    onScroll () {
      const currentScrollPosition = window.pageYOffset || document.documentElement.scrollTop
      if (currentScrollPosition < 0) {
        return
      }
      // Stop executing this function if the difference between
      // current scroll position and last scroll position is less than some offset
      if (Math.abs(currentScrollPosition - this.lastScrollPosition) < 60) {
        return
      }
      this.showFlatButton = currentScrollPosition > this.lastScrollPosition
      this.lastScrollPosition = currentScrollPosition
    }
  },
  mounted() {
    window.addEventListener('scroll', this.onScroll)
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background: rgb(29,34,48);
  background: -webkit-linear-gradient(90deg, rgba(29,34,48,1) 0%, rgba(28,33,47,1) 11%, rgba(24,30,42,1) 61%, rgba(24,30,42,1) 65%);
  user-select: none;
  position: relative;
}
#app {
    overflow: hidden;
  font-family: 'Raleway';
}

.bold {
  font-weight: 700
}

.size-15 {
  font-size: 15px
}

.content-wrap {
   /* background-image:  url('./assets/images/bg-curvy-desktop.svg');
    background-size: contain;
    background-repeat: no-repeat; */
}

.responsive-img {
  height: auto;
  width: 100%;
}

.size-16 {
  font-size: 16px
}

.size-35 {
  font-size: 35px
}

.y-20 {
  margin-top: 20px
}

.white {
  color: white;
}

.avatar {
  border-radius: 50%;
  width: 30px;
  height: 30px;
  margin-right: 10px
}

</style>
