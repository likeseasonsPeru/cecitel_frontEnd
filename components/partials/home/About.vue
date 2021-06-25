<template>
  <div class="About">
    <b-container>
      <b-row>
        <b-col md="6">
          <div>
            <img
              src="@/assets/img/girl_1.png"
              class="mx-auto d-block img-fluid"
              alt="girl_read"
            />
          </div>
        </b-col>
        <b-col md="6" class="text-md-left">
          <div>
            <h4 class="mb-4">
              Valoramos la confianza puesta <br />
              en nosotros y estamos cerca de <br />
              ti para el autodescubrimiento <br />
              de tus talentos y sueños.
            </h4>
            <p>
              Creamos experiencias de aprendizaje creativas <br />
              intuitivas, fortalecidas por la cercanía en el trato y<br />
              el diálogo, compartiendo conocimientos teóricos y <br />
              practicos.
            </p>
            <b-button class="px-4" pill>Ver más</b-button>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'About',
}
</script>

<style lang="css" scoped>
.About {
  background-color: #fff;
}
</style>
