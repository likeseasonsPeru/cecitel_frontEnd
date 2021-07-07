<template>
  <b-modal id="modal-center" class="Modal" hide-header hide-footer>
    <div class="ModalLogin">
      <h1 class="ModalLogin__title">Bienvenido</h1>
      <div class="ModalLogin__form">
        <h6 class="ModalLogin__form-label">Correo Electrónico</h6>
        <b-form-group id="input-group-1" label-for="input-1">
          <b-form-input id="input-1" type="email" required></b-form-input>
        </b-form-group>
        <h6 class="ModalLogin__form-label">Contraseña</h6>
        <b-form-group id="input-group-2" label-for="input-2">
          <b-form-input id="input-2" type="password" required></b-form-input>
        </b-form-group>
      </div>
      <div class="ModalLogin__settings">
        <a class="ModalLogin__settings-a">¿Olvidaste tu contraseña?</a>
        <b-button pill block class="ModalLogin__settings-button my-4"
          >Iniciar Sesión</b-button
        >
        <span class="ModalLogin__settings-register"
          >¿Aún no tienes una cuenta?
          <button class="ModalLogin__settings-register-button">
            Regístrate
          </button></span
        >
      </div>
    </div>
  </b-modal>
</template>

<script>
export default {
  name: 'ModalLogin',
  form: {
    email: '',
    password: '',
  },
}
</script>

<style scoped>
.Modal {
  border: none;
  border-radius: 50px;
}
.ModalLogin {
  padding: 35px 30px;
  color: #568ae9;
}
.ModalLogin__title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
}
.ModalLogin__form-label {
  font-weight: normal;
  font-size: 24px;
  line-height: 36px;
}
.ModalLogin__settings {
  text-align: center;
}
.ModalLogin__settings-button {
  background: #568ae9;
  border: none;
  border-radius: 40px;
  color: #fff;
  font-size: 30px;
  font-weight: bold;
  line-height: 45px;
}
.ModalLogin__settings-a {
  font-size: 21px;
  line-height: 31px;
  cursor: pointer;
  text-decoration-line: underline;
}
.ModalLogin__settings-register {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
}
.ModalLogin__settings-register-button {
  background: none;
  border: none;
  color: #568ae9;
  font-weight: bold;
  text-decoration-line: underline;
}
</style>
