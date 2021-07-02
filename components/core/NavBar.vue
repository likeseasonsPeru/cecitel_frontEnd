<template>
  <b-navbar class="Navbar" toggleable="lg" type="dark">
    <b-container>
      <b-navbar-brand href="/">
        <div>
          <img
            :src="require('@/components/svg/logos/logo-navbar.svg')"
            alt="Logo Cecitel"
            class="d-inline-block align-left"
          />
        </div>
      </b-navbar-brand>

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
            <template slot="button-content"> Corporativo </template>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/coaching"
            >
              Coaching
            </b-dropdown-item>
            <b-dropdown-item
              class="navbar__subMenu text-capitalize"
              to="/televentas"
            >
              Televentas
            </b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item href="/corporativo">Corporativo</b-nav-item>
          <b-nav-item href="/conocenos">Conócenos</b-nav-item>
          <b-nav-item href="/contactanos">Contáctanos</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav>
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mx-4 form-input"
              placeholder="Buscar"
            ></b-form-input>
          </b-nav-form>

          <span
            ><img
              :src="require('~/components/svg/icons/heartnav.svg')"
              alt="icon heart"
              class="mx-2"
          /></span>
          <span
            ><img
              :src="require('~/components/svg/icons/shopnav.svg')"
              alt="icon shop"
              class="mx-2"
          /></span>
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
  background-color: #222;
}
.form-input {
  background-color: #222;
  border: 1px solid #fff;
  border-radius: 15px;
  color: #fff;
}
</style>
