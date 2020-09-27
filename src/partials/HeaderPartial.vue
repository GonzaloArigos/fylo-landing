<template>
  <nav style="color:black" class="navbar navbar-light fixed-top navbar-expand-xl dark-transparent">
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
        <li v-scroll-to="'.offer'" class="nav-item">
          <a href="#" class="nav-link active">
            <strong>Quiénes somos</strong>
          </a>
        </li>
        <li v-scroll-to="'.services'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Qué hacemos</strong>
          </a>
        </li>
        <li v-scroll-to="'.reviews'" class="nav-item active">
          <a href="#" class="nav-link">
            <strong>Nosotros</strong>
          </a>
        </li>
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
  border-bottom: 2px solid #46d4dc; 
  /* background: #cbcbcb5e; */
}
</style>
