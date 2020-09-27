<template>
  <nav class="navbar navbar-light navbar-expand-xl dark-transparent">
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="text-black navbar-toggler-icon"></span>
    </button>

    <a class="navbar-brand p-2 pl-3" href="#">
      <img
        width="130"
        src="./../../public/images/logo.png"
        class="img-fluid mb-0 mt-2"
        alt="Responsive image"
      />
    </a>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li v-scroll-to="'.offer'" class="nav-item tex-raviol">
          <a href="#" class="nav-link active">
            <strong>Productos</strong>
          </a>
        </li>
        <li v-scroll-to="'.services'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Linea vegana</strong>
          </a>
        </li>
        <!-- <li v-scroll-to="'.reviews'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Nosotros</strong>
          </a>
        </li> -->
        <li v-scroll-to="'.contact'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Contactanos</strong>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style>
.dark-transparent {
  background: #ffffff;
  border-bottom: 2px solid #e91e28; 
  /* background: #cbcbcb5e; */
}
.text-raviol{
  color: #e91e28 !important;
}
</style>
