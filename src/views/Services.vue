<template>
  <div class="services container mt-4">
    <h2 class="text-center">Nuestra</h2>
    <h2 class="text-center">
      LINEA
      <span class="vegana-text bold"
        >| VEGANA <i class="fas fa-seedling vegana-text"></i
      ></span>
    </h2>

    <div class="services-group">
      <div data-aos="fade" class="services-group-item">
        <div>
          <img
            class="rounded-circle"
            height="200"
            width="250"
            src="./../../public/images/sorrent.png"
            alt
          />
        </div>
        <div class="y-20 item-description">
          <h3 class="bold vegana-text">Sorrentinos</h3>
          <br />
          <h5><i class="fas fa-seedling vegana-text"></i> Muzzarella y jamón ahumado</h5>
          <h5><i class="fas fa-seedling vegana-text"></i>  Calabaza y muzzarella</h5>
        </div>
      </div>
      <div data-aos="fade" class="services-group-item">
        <div>
          <img
            class="rounded-circle"
            height="200"
            width="250"
            src="./../../public/images/ravioles-vegana.jpg"
            alt
          />
        </div>
        <div class="y-20 item-description">
          <h3 class="bold vegana-text">Ravioles</h3>
          <br />
          <h5><i class="fas fa-seedling vegana-text"></i>  Verdura y soja</h5>
          <h5><i class="fas fa-seedling vegana-text"></i>  Tofu y nuez</h5>
          <h5><i class="fas fa-seedling vegana-text"></i>  Tofu, nuez, jamón</h5>
          <h5><i class="fas fa-seedling vegana-text"></i>  Tofu, nuez, verdura</h5>
        </div>
      </div>
      <div data-aos="fade" class="services-group-item">
        <div>
          <img
            class="rounded-circle"
            height="200"
            width="250"
            src="./../../public/images/muchomas.jpg"
            alt
          />
        </div>
        <div class="y-20 item-description">
          <h3 class="bold vegana-text">Y muchos más!</h3>
          <br />
          <h5><i class="fas fa-seedling vegana-text"></i> Ñoquis</h5>
          <h5><i class="fas fa-seedling vegana-text"></i> Tapa mini tarta integral</h5>
          <h5><i class="fas fa-seedling vegana-text"></i> Tapa empanada integral</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
* {
  color: black;
  text-align: center;
}

.vegana-text {
  color: green !important;
}

.services {
  display: flex;
  flex-direction: column;
}

.services-group {
  display: flex;
  flex-direction: row;
}

.services-group-item {
  display: flex;
  flex-direction: column;
  padding: 30px;
  border-bottom: 2px solid #e91e28;
}

@media (min-width: 768px) and (max-width: 1024px) {
  .services {
    padding: 0;
  }

  .services-group {
    flex-direction: column;
    padding-top: 40px;
  }

  .services-group-item {
    padding: 20px;
  }

  .item-description span:first-of-type {
    font-size: 20px;
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
  .services {
    padding: 0;
  }

  .services-group {
    flex-direction: column;
    padding-top: 40px;
  }

  .services-group-item {
    padding: 20px;
  }

  .item-description span:first-of-type {
    font-size: 20px;
  }
}

@media (min-width: 481px) and (max-width: 767px) {
  .services {
    padding: 0;
  }

  .services-group {
    flex-direction: column;
    padding-top: 40px;
  }

  .item-description span:first-of-type {
    font-size: 20px;
  }

  .services-group-item {
    padding: 20px;
  }
}

@media (min-width: 320px) and (max-width: 480px) {
  .services {
    padding: 0;
  }

  .services-group {
    flex-direction: column;
    padding-top: 40px;
  }

  .item-description span:first-of-type {
    font-size: 20px;
  }

  .services-group-item {
    padding: 20px;
  }
}
</style>

