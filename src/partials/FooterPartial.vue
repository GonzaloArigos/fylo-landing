<template>
  <div class="footer contact">
    <div id="footer-about">
      <div id="logo">
        <img
          width="130"
          class="img-fluid logo-nav"
          src="./../../public/images/logo.png"
          alt
        />
      </div>
      <div class="mt-2" id="footer-text">
        <h5>Horarios de atención:</h5>
        <p>Martes a sábados: de 8:30hs a 13hs y 17hs a 19hs</p>
        <p>Domingos: de 8:30hs a 13.20hs</p>
        <p>Lunes: cerrados</p>
        <p>Alvear 2125 Villa Ballester</p>
      </div>
    </div>
    <div id="footer-contact">
      <div class="links-list">
        <ul>
          <li>
            <h5 class="text-success">
              <i class="fab fa-whatsapp text-success"></i> Pedinos por WhatsApp!
            </h5>
          </li>

          <li>
            <div>
              <a href="http://wa.link/lcverc" target="_blank" class>
                <button class="btn btn-success">
                  <h5 class="text-white">
                    <i class="fab fa-whatsapp text-white"></i> 114738-3570
                  </h5>
                </button>
              </a>
            </div>
            <div class="mt-2">
              <a
                href="https://order.ubereats.com/buenos-aires/food-delivery/%F0%9F%9B%92%20Que%20Ravioles/ehzBmu7KTLCrdQPwh14usQ/?utm_source=web-restaurant-manager"
                rel="noopener noreferrer"
                target="_blank"
              >
                <button class="btn btn-dark">
                  <h5 class="text-white">
                    <i class="fab fa-uber"></i> Uber Eats
                  </h5>
                </button>
              </a>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="links-list">
      <ul>
        <li><i class="fas fa-hashtag"></i> Nuestras redes</li>
        <li v-on:click="irAIg()">
          <i class="fab fa-instagram ig"></i> queravioles.alvear
        </li>
      </ul>
      <hr />
      <a href="http://ggsolutionsweb.ml">
        <small
          >Sitio web creado por ggsolutionsweb, seguinos en instragram
          @ggsolutionsweb</small
        >
      </a>
    </div>
  </div>
</template>
<script>
export default {
  methods: {
    irAIg() {
      window.location.href = "https://instagram.com/queravioles.alvear";
    },
  },
};
</script>
<style scoped>
.ig {
  color: #d04977;
}
a:hover {
  color: white;
  text-decoration: none;
}
* {
  color: black;
}
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-grow: 1;
  background: #ffffff;
  border-top: 5px solid #e91e28;
}
.footer-about {
  display: flex;
  flex-direction: column;
  flex-grow: 2;
}

ul {
  list-style: none;
}

ul > li {
  padding-top: 20px;
  cursor: pointer;
}

@media (min-width: 768px) and (max-width: 1024px) {
  .footer {
    flex-direction: column;
    padding: 100px 50px 100px 50px;
    align-items: flex-start;
  }

  ul {
    padding: 0;
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
  .footer {
    flex-direction: column;
    padding: 100px 50px 100px 50px;
    align-items: flex-start;
  }

  ul {
    padding: 0;
  }
}

@media (min-width: 481px) and (max-width: 767px) {
  .footer {
    flex-direction: column;
    padding: 100px 50px 100px 50px;
    align-items: flex-start;
  }

  ul {
    padding: 0;
  }
}

@media (min-width: 320px) and (max-width: 480px) {
  .footer {
    flex-direction: column;
    padding: 100px 50px 100px 50px;
    align-items: flex-start;
  }

  ul {
    padding: 0;
  }
}
</style>

