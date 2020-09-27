<template>
  <div class="footer">
    <div id="footer-about">
      <!-- <div id="logo">
        <img
          width="230"
          class="img-fluid logo-nav"
          src="./../../public/images/logo.png"
          alt
        />
      </div>
      <div id="footer-text">
        <p>
          Seguinos en instagram y enterate de todo lo nuevo.
          <br />2020 <br />Buenos Aires, Argentina
        </p>
      </div> -->
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
            <a href="http://wa.link/lcverc" target="_blank" class>
              <button class="btn btn-success">
                <h5 class="text-white">
                  <i class="fab fa-whatsapp"></i> 114738-3570
                </h5>
              </button>
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="links-list">
      <ul>
        <li><i class="fas fa-hashtag"></i> Nuestras redes</li>
        <li v-on:click="irAIg()">
          <i class="fab fa-instagram ig"></i> Instagram
        </li>
      </ul>
      <small
        >Sitio web creado por ggsolutionsweb, seguinos en instragram
        @ggsolutionsweb</small
      >
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
  padding: 100px 50px 100px 50px;
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

