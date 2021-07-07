<template>
  <b-modal id="modal-register" class="Modal" hide-header hide-footer>
    <div class="ModalLogin">
      <h1 class="ModalLogin__title">Únete a Cecitel</h1>
      <div class="ModalLogin__form">
        <h6 class="ModalLogin__form-label">Nombre de usuario</h6>
        <b-form-group id="input-group-1" label-for="input-1">
          <b-form-input id="input-1" type="text" required></b-form-input>
        </b-form-group>
        <h6 class="ModalLogin__form-label">Correo electrónico</h6>
        <b-form-group id="input-group-2" label-for="input-2">
          <b-form-input id="input-2" type="email" required></b-form-input>
        </b-form-group>
        <h6 class="ModalLogin__form-label">Número de DNI</h6>
        <b-form-group id="input-group-3" label-for="input-3">
          <b-form-input id="input-3" type="number" required></b-form-input>
        </b-form-group>
        <h6 class="ModalLogin__form-label">Contraseña</h6>
        <b-form-group id="input-group-4" label-for="input-4">
          <b-form-input id="input-4" type="password" required></b-form-input>
        </b-form-group>
        <h6 class="ModalLogin__form-label">Ingresa la contraseña nuevamente</h6>
        <b-form-group id="input-group-5" label-for="input-5">
          <b-form-input id="input-5" type="password" required></b-form-input>
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
  name: 'ModalRegister',
}
</script>
