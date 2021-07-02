<template>
  <div>
    <b-row class="mt-3 dark-grey-text d-flex justify-content-center">
      <b-col md="2" lg="2" xl="2">
        <div>
          <div class="pb-2">
            <img
              :src="require('@/components/svg/logos/logo-footer.svg')"
              alt="Logo Cecitel"
              class="d-inline-block align-left"
            />
          </div>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2">
        <div>
          <div class="pb-2">Síguenos</div>
          <b-link
            id="facebook"
            href="https://www.facebook.com/Cecitel/"
            target="_blank"
            class="circle"
          >
            <!-- <label class="text-hide" for="facebook">Facebook</label> -->
            F
          </b-link>
          <b-link
            id="facebook"
            href="https://www.instagram.com/cecitel.pe/"
            target="_blank"
            class="circle"
          >
            <!-- <label class="text-hide" for="facebook">Facebook</label> -->
            I
          </b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2" class="mb-2 text-capitalize">
        <div class="d-block">
          <div class="pb-2">Cursos y más</div>
          <b-link>Semipresenciales</b-link>
          <b-link>Enlatados</b-link>
          <b-link>Corporativo</b-link>
          <b-link>Coaching</b-link>
        </div>
      </b-col>
      <b-col md="2" lg="2" xl="2" class="mb-2 text-capitalize">
        <div class="d-block">
          <div class="pb-2">Contáctanos</div>
          <b-link>Dirección</b-link>
          <b-link>Control Telefónico</b-link>
          <b-link>Correo</b-link>
        </div>
      </b-col>
    </b-row>
    <b-row class="mt-3 dark-grey-text d-flex justify-content-center">
      <b-col md="4" lg="4" xl="4">
        <div>
          <span>Copyright - 2021</span>
        </div>
      </b-col>
      <b-col md="4" lg="4" xl="4">
        <div class="d-flex">
          <b-link>Términos y Condiciones</b-link>
          <b-link>Politicas de protección de datos</b-link>
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
