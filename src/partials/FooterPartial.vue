<template>
  <div class="footer">
    <div id="footer-about">
      <div id="logo">
        <img width="230" class="img-fluid logo-nav" src="./../../public/images/logo.png" alt />
      </div>
      <div id="footer-text">
        <p>
          Seguinos en instagram y enterate de todo lo nuevo.
          <br />2020
          <br />Buenos Aires, Argentina
        </p>
      </div>
    </div>
    <div id="footer-contact">
      <!-- <div><span>+1-543-123-4567</span></div> -->
      <div class="links-list">
        <ul>
          <li>
            <i class="far fa-envelope"></i> Mail de contacto
          </li>

          <li>
            <a href="mailto:ggsolutionsweb@gmail.com" target="_blank" class>ggsolutionsweb@gmail.com</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="links-list">
      <ul>
        <li>
          <i class="fas fa-hashtag"></i> Nuestras redes
        </li>
        <li v-on:click="irAIg()">
          <i class="fab fa-instagram ig"></i> Instagram
        </li>
      </ul>
    </div>

    <div id="footer-social-networks"></div>
  </div>
</template>
<script>
export default {
  methods: {
    irAIg() {
      window.location.href = "https://instagram.com/ggsolutionsweb";
    }
  }
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
  border-top: 2px solid #49cbd3;
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

