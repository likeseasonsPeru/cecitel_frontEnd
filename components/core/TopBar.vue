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
          <span class="TopBar__log pr-3">Ingresar</span>
          <span class="TopBar__sign ml-3">Registrate</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopBar',
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
  color: #7ddddd;
  border-right: 1px solid #a6a6a6;
}
.TopBar__sign {
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  color: #7ddddd;
}
</style>
