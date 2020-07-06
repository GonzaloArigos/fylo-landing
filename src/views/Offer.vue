<template>
  <div class="offer mt-4">
    <div data-aos="fade-right p-3">
      <img
        class="responsive-img"
        src="../assets/images/illustration-stay-productive.png"
        alt="stay productive with fylo"
      />
    </div>
    <div data-aos="fade-left" id="offer-info">
      <div class="pl-4 pr-4">
        <span class="bold white size-35">
          Soluciones a medida,
          <br />calidad y capacitación
        </span>
      </div>
      <br />
      <div class="pl-4 pr-4">
        <span
          class="white"
        >GG design esta centrado exclusivamente en el cliente, su crecimiento es nuestra meta.</span>
        <br />
        <br />
        <span
          class="white"
        >Seleccionaremos la mejor solución de software para que su negocio crezca y lo capacitaremos para que se vuelva un experto!</span>
       
      </div>
    </div>
  </div>
</template>

<style>
.offer {
  display: flex;
  text-align: left;
  justify-content: center;
  align-items: center;
}

.offer-info {
  display: flex;
}

#link-fylo-work {
  color: hsl(176, 68%, 64%);
}

@media (min-width: 768px) and (max-width: 1024px) {
  .offer {
    flex-direction: column;
  }

  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
  .offer {
    flex-direction: column;
  }

  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 481px) and (max-width: 767px) {
  .offer {
    flex-direction: column;
  }

  #offer-info {
    padding-top: 40px;
  }
}

@media (min-width: 320px) and (max-width: 480px) {
  .offer {
    flex-direction: column;
  }

  #offer-info {
    padding-top: 40px;
  }
}
</style>

