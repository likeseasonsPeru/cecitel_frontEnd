<template>
  <div class="TopBar">
    <div class="container">
      <div class="TopBar__content">
        <div>
          <span class="mr-3"
            ><img
              :src="require('~/components/svg/icons/fbnav.svg')"
              alt="icon facebook"
          /></span>
          <span
            ><img
              :src="require('~/components/svg/icons/instanav.svg')"
              alt="icon instagram"
          /></span>
        </div>
        <div>
          <button v-b-modal.modal-center class="TopBar__log pr-3">
            Ingresar
          </button>
          <ModalLogin />
          <button v-b-modal.modal-register class="TopBar__sign ml-3">
            Registrate
          </button>
          <ModalRegister />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ModalLogin from '~/components/partials/modals/ModalLogin.vue'
import ModalRegister from '~/components/partials/modals/ModalRegister.vue'
export default {
  name: 'TopBar',
  components: { ModalLogin, ModalRegister },
}
</script>
<style scoped>
.TopBar {
  background-color: #222;
  height: 50px;
  width: 100%;
}
span {
  color: #fff;
}
.TopBar__content {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #a6a6a6;
  padding: 9px 0;
}
.TopBar__log {
  font-size: 21px;
  line-height: 31px;
  border: none;
  color: #7ddddd;
  border-right: 1px solid #a6a6a6;
  background: none;
}
.TopBar__sign {
  border: none;
  background: none;
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  color: #7ddddd;
}
</style>
