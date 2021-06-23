<template>
  <div class="TopBar">
    <div class="container">
      <div class="d-flex space-beetween">
        <div>
          <span>F</span>
          <span>I</span>
        </div>
        <div>
          <span>Ingresar</span>
          <span>Registrate</span>
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
.container {
  min-height: 50px !important;
}
span {
  color: #fff;
}
</style>
