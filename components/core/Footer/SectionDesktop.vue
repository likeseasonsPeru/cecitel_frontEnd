<template>
  <div class="Footer py-5">
    <b-row class="mt-3 dark-grey-text d-flex justify-content-center">
      <b-col md="2" lg="2" xl="2">
        <div>
          <div class="pb-2">
            <img
              :src="require('@/components/svg/logos/logo-footer.svg')"
              alt="Logo Cecitel"
              class="img-fluid"
            />
          </div>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2" class="text-center">
        <div>
          <div class="Footer-direc pb-2">Síguenos</div>
          <b-link
            id="facebook"
            href="https://www.facebook.com/Cecitel/"
            target="_blank"
            class="circle mx-2"
          >
            <img
              :src="require('@/components/svg/icons/fb-footer.svg')"
              alt="facebook"
              class="Footer-img"
            />
          </b-link>
          <b-link
            id="instagram"
            href="https://www.instagram.com/cecitel.pe/"
            target="_blank"
            class="circle mx-2"
          >
            <img
              :src="require('@/components/svg/icons/insta-footer.svg')"
              alt="instagram"
              class="Footer-img"
            />
          </b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2" class="mb-2 text-capitalize">
        <div class="Footer-nav">
          <div class="Footer-direc pb-2">Cursos y más</div>
          <b-link>Semipresenciales</b-link>
          <b-link>Enlatados</b-link>
          <b-link>Corporativo</b-link>
          <b-link>Coaching</b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2" class="mb-2 text-capitalize">
        <div class="Footer-nav">
          <div class="Footer-direc pb-2">Contáctanos</div>
          <b-link>Dirección</b-link>
          <b-link>Control Telefónico</b-link>
          <b-link>Correo</b-link>
        </div>
      </b-col>
    </b-row>
    <b-row class="mt-3 dark-grey-text d-flex justify-content-center">
      <b-col md="4" lg="4" xl="4">
        <div>
          <b-link>Copyright</b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2">
        <div class="Footer-terms text-center">
          <b-link href="/terminos-y-condiciones">Términos y condiciones</b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2">
        <div class="text-center">
          <b-link href="/politicas">Politicas de protección de datos</b-link>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: 'SectionDesktop',
}
</script>

<style lang="css" scoped>
/* .Footer {
} */
.Footer-img {
  width: 45px;
}
.Footer-nav {
  display: flex;
  flex-direction: column;
}
.Footer-direc {
  font-weight: bold;
  font-size: 24px;
  line-height: 30px;
  color: #fff;
}
a {
  color: #fff;
  font-weight: 200;
  text-decoration: none;
}
.Footer-terms {
  border-right: 1px solid #fff;
}
</style>
