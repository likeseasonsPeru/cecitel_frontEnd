<template>
  <b-navbar class="Navbar" toggleable="lg" type="dark">
    <b-container>
      <b-navbar-brand href="#">CECITEL</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item-dropdown>
            <template slot="button-content">
              Cursos y más
              <span style="font-size: 12px">
                <chevron-down-icon />
              </span>
            </template>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/online"
            >
              Online
            </b-dropdown-item>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/semipresenciales"
            >
              Semipresenciales
            </b-dropdown-item>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/webinars"
            >
              Webinars
            </b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown>
            <template slot="button-content">
              Corporativo
              <span style="font-size: 12px">
                <chevron-down-icon />
              </span>
            </template>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/online"
            >
              Coaching
            </b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item href="/corporativo">Corporativo</b-nav-item>
          <b-nav-item href="/conocenos">Conócenos</b-nav-item>
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
