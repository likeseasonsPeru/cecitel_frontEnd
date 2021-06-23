<template>
  <b-navbar class="Navbar" toggleable="lg" type="dark">
    <b-container>
      <b-navbar-brand href="#">CECITEL</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Cursos y más</b-nav-item>
          <b-nav-item href="#">Webinars</b-nav-item>
          <b-nav-item href="#">Conócenos</b-nav-item>
          <b-nav-item href="#">Contáctanos</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mr-sm-2 form-input"
              placeholder="Buscar"
            ></b-form-input>
          </b-nav-form>

          <b-nav-item href="#">c</b-nav-item>
          <b-nav-item href="#">C</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-container>
  </b-navbar>
</template>
<script>
export default {
  name: 'NavBar',
}
</script>
<style lang="css">
.Navbar {
  height: 50px;
  background-color: #222;
}
.form-input {
  background-color: #222;
  border: 1px solid #fff;
  border-radius: 15px;
  color: #fff;
}
</style>
