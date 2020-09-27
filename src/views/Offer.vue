<template>
  <div class="offer text-black gradient">

    <div data-aos="fade-left" class="pqnosotros firstback text-center">
      <div class="w3-center w3-margin-bottom">
        <div class="pt-5">
          <h2 class="bold">NUESTRA MISION</h2>
          <small class="text-center bold">Somos especialistas en desarrollo de software.</small>
        </div>
        <div class="text-who-is box p-1">
          <h1>
            <i class="fas fa-check-circle brand-color"></i>
          </h1>
          <h5>
            <div class>
              "Apuntamos a la
              <b>creación</b> de alto impacto,
              <br />generando
              <b>soluciones de software</b>
              <br />y diseño a medida para cada
              <b>cliente</b>"
            </div>
          </h5>
        </div>
      </div>
    </div>

    <div data-aos="fade-left" class="pqnosotros firstback text-center">
      <div class="w3-center w3-margin-bottom">
        <div class="pt-5">
          <h2 class="bold">¿QUÉ BUSCAMOS?</h2>
        </div>
        <div class="text-who-is box p-1">
          <h1>
            <i class="fas fa-search-dollar brand-color"></i>
          </h1>
          <h5>
            <div class>
              <div class="white">Queremos que te animes a <b>dar el salto.</b></div>
              <div class="white">Te acompañaremos dando la mejor solución <b>de software.</b></div>
              <div
                class="white"
              >Nos centramos exclusivamente en cada <b>cliente</b> con capacitación y apuntando al <b>crecimiento</b> del negocio.</div>
            </div>
          </h5>
        </div>
      </div>
    </div>

    <div data-aos="fade-left" class="pqnosotros firstback text-center p-5">
      <button v-scroll-to="'.services'" class="btn btn-info">Ver servicios</button>
    </div>
  </div>
</template>

<style>
.brand-color{
  color: #46d4dc;
}
.gradient {
  height: 100%;
  /* background: linear-gradient(to right, #46d4dc, #46d4dc) */
}

.bordered {
  border-top: 10px solid #c7a511;
  /* border-bottom: 10px solid #c7a511; */
}
.box {
  background: linear-gradient(to right, #9696960a, #cabd770f);
  border: 1px solid #46d4dc;
  border-radius: 3%;
}
.lamp {
  color: #c7a511;
}
.transparent-box {
  background: #0000005c;
  border-radius: 10px;
  text-decoration: overline;
}

.text-who-is {
  letter-spacing: 2px;
}

.pqnosotros {
  margin: 0 10% 0% 10%;
  padding: 5%;
}

.offer-info {
  display: flex;
}

@media (min-width: 768px) and (max-width: 1024px) {
  .pqnosotros {
    margin: 0 5% 0% 5%;
    padding: 5%;
  }
  .fullcenter {
    padding: 5% 5%;
    text-align: center;
  }
  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
  .pqnosotros {
    margin: 0 5% 0% 5%;
    padding: 5%;
  }
  .fullcenter {
    padding: 5% 5%;
    text-align: center;
  }
  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 481px) and (max-width: 767px) {
  .pqnosotros {
    margin: 0 5% 0% 5%;
    padding: 5%;
  }
  .fullcenter {
    padding: 5% 5%;
    text-align: center;
  }
  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 320px) and (max-width: 480px) {
  .pqnosotros {
    /* margin: 0 5% 0% 5%; */
    /* padding: 0.5%; */
  }

  #offer-info {
    padding-top: 40px;
  }
}
</style>

