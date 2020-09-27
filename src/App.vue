<template>
  <div id="app">
    <Header />

    <Home />
    <Offer />
    <Services />

    <Reviews />
    <Contact />

    <Footer />
    <!-- <MobileMenu /> -->

    <FloatButton v-if="showFlatButton" />
  </div>
</template>

<script>
import Footer from "./partials/FooterPartial.vue";
import Header from "./partials/HeaderPartial.vue";
import Home from "./views/Home";
import Services from "./views/Services";
import Offer from "./views/Offer";
import Reviews from "./views/Reviews";
import Contact from "./views/Contact";
import FloatButton from "./components/FloatButton";

export default {
  name: "app",
  components: {
    Header,
    Footer,
    Home,
    Services,
    Offer,
    Reviews,
    Contact,
    FloatButton
  },
  data() {
    return {
      showFlatButton: false,
      lastScrollPosition: 0
    };
  },
  methods: {
    onScroll() {
      const currentScrollPosition =
        window.pageYOffset || document.documentElement.scrollTop;
      if (currentScrollPosition < 0) {
        return;
      }
      // Stop executing this function if the difference between
      // current scroll position and last scroll position is less than some offset
      if (Math.abs(currentScrollPosition - this.lastScrollPosition) < 60) {
        return;
      }
      this.showFlatButton = currentScrollPosition > this.lastScrollPosition;
      this.lastScrollPosition = currentScrollPosition;
    }
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  }
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  user-select: none;
  position: relative;
}
#app {
font-family: "Montserrat", sans-serif
}

.bold {
  font-weight: 700;
}

.size-15 {
  font-size: 15px;
}

.sticky {
  position: -webkit-sticky; /* Safari */
  position: sticky;
  top: 0;
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
  font-size: 16px;
}

.size-35 {
  font-size: 35px;
}

.y-20 {
  margin-top: 20px;
}


.avatar {
  border-radius: 50%;
  width: 80px;
  height: 80px;
  margin-right: 10px;
}
</style>
