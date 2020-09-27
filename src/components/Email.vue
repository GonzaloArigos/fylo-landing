<template>
  <div data-aos="zoom-in" class="email text-white">
    <div>
      <span class="bold white size-35 email-title">Solicitar asesoramiento</span>
    </div>
    <br />
    <div>
      <span class="white">Indicanos de que se trata tu negocio y te diremos la mejor solución</span>
    </div>
    <br />

    <div class="input-group">
      <textarea
        placeholder="Estimados, me gustaria consultar por..."
        class="form-control"
        aria-label="With textarea"
        v-model="emailBody"
      ></textarea>
    </div>
    <div>
      <a
        :href="'mailto:ggsolutionsweb@gmail.com?subject=Solicitud de asesoramiento&body=' + emailBody"
        class="btn btn-primary btn-lg mt-4"
      ><i class="far fa-paper-plane"></i> Enviar mail</a>
    </div>

    <!-- <Button>Solicitar!</Button> -->

    <small v-on:click="irAIg()" class="text-left mt-3">
      Recuerda que también atendemos consultas por &nbsp;
      <i class="fab fa-instagram ig"></i> Instagram.
    </small>
  </div>
</template>

<script>
import Button from "../components/Button";
export default {
  data() {
    return {
      emailBody: ""
    };
  },
  components: {
    Button
  },
  methods: {
    irAIg() {
      window.location.href = "https://instagram.com/ggsolutionsweb";
    }
  }
};
</script>


<style>
.ig {
  color: #d04977;
}
.email {
  display: flex;
  width: 50%;
  border-radius: 5px;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  padding: 40px;
  align-items: center;
  background: #49cbd3;

  cursor: pointer;
  -webkit-box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
  -moz-box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
  box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
}

.inputAndButton {
  width: 100%;
  display: flex;
}

#input-wrapper {
  flex-grow: 11;
}

#button-wrapper {
  flex-grow: 1;
}

#email-input {
  width: 100%;
  height: 45px;
  border-radius: 100px;
  outline: none;
  border: none;
}

@media (min-width: 768px) and (max-width: 1024px) {
  .email {
    width: 100%;
  }

  .email-title {
    font-size: 20px !important;
  }

  .inputAndButton {
    flex-direction: column;
  }

  #input-wrapper {
    margin-bottom: 20px;
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
  .email {
    width: 100%;
  }

  .email-title {
    font-size: 20px !important;
  }

  .inputAndButton {
    flex-direction: column;
  }

  #input-wrapper {
    margin-bottom: 20px;
  }
}

@media (min-width: 481px) and (max-width: 767px) {
  .email {
    width: 100%;
  }

  .email-title {
    font-size: 20px !important;
  }

  .inputAndButton {
    flex-direction: column;
  }

  #input-wrapper {
    margin-bottom: 20px;
  }
}

@media (min-width: 320px) and (max-width: 480px) {
  .email {
    width: 100%;
  }

  .email-title {
    font-size: 20px !important;
  }

  .inputAndButton {
    flex-direction: column;
  }

  #input-wrapper {
    margin-bottom: 20px;
  }
}
</style>

