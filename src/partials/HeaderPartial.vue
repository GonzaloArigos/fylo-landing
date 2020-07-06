<template>

  <nav

    class="navbar fixed-top navbar-expand-xl navbar-dark dark-transparent"
  >
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <a class="navbar-brand p-2 pl-3" href="#">
      <img width="200" src="../assets/logo.png" class="img-fluid mb-0 mt-2" alt="Responsive image" />
    </a>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li v-scroll-to="'.services'" class="nav-item">
          <a href="#" class="nav-link active">
            <strong>Servicios</strong>
          </a>
        </li>
        <li v-scroll-to="'.offer'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Beneficios</strong>
          </a>
        </li>
        <li v-scroll-to="'.reviews'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Nosotros</strong>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style>
.dark-transparent {
 background: #00000075;
}
</style>
