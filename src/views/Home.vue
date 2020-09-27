<template>
  <div
    id="carouselExampleIndicators"
    class="home carousel slide"
    data-ride="carousel"
  >
    <div class="carousel-inner" role="listbox">
      <!-- Slide One - Set the background image for this slide in the line below -->
      <div class="carousel-item active firstitem">
        <div class="carousel-caption">
          <h2 class="display-3 text-raviol">Pastas Que Ravioles</h2>
          <h4>
            <span class="text-raviol-subtitle">
              Fabrica de pastas artesanales</span
            >
          </h4>

          <div class="caracteristicas p-2 mt-1">
            <h5>
               <span class="text-raviol-sm"> Productos 100% naturales.</span>
            </h5>
            <h5>
              <span class="text-raviol-sm">
                Elaboración diaria y artesanal.</span
              >
            </h5>
            <h5>
              <span class="text-raviol-sm"> Pastas veganas</span>
            </h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {},
};
</script>


<style scoped>
.light-blue {
  background: #008effbf;
}
.firstitem {
  background-image: url("./../../public/images/portada.jpg") !important;
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
.caracteristicas {
    background: #d0bbae80;
    border-radius: 3%;
}
</style>

