<template>
  <div id="carouselExampleIndicators" class="home carousel slide" data-ride="carousel">

    <div class="carousel-inner" role="listbox">
      <!-- Slide One - Set the background image for this slide in the line below -->
      <div class="carousel-item active firstitem">
        <div class="carousel-caption">
          <h2 class="display-4">Dá el salto.</h2>
          <p class="lead">Alcanzá tus objetivos de marca dando el salto, con nosotros.</p>
          <button v-scroll-to="'.contact'" class="btn btn-info">Asesorate</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {}
};
</script>


<style scoped>
.light-blue{
  background: #008effbf;
}
.firstitem {
  background-image: url("https://images.pexels.com/photos/669996/pexels-photo-669996.jpeg?cs=srgb&dl=black-laptop-beside-black-computer-mouse-inside-room-669996.jpg&fm=jpg") !important;
}
.seconditem {
  background-image: url("https://www.pexels.com/photo/4665064/download/") !important;
}
.carousel-item {
  height: 100vh;
  min-height: 350px;
  background: no-repeat center center scroll;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
</style>

