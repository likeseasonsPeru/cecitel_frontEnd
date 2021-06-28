<template>
  <div class="AboutUs">
    <BannerTop :image="image" />
    <div class="AboutUs-fond">
      <b-container>
        <p class="AboutUs-fond__text">
          Creamos experiencias de aprendizaje creativas, intuitivas,
          fortalecidas por la cercanía en el trato, en el diálogo y en el
          compartir de conocimientos teóricos y prácticos.
        </p>
      </b-container>
    </div>
    <b-container>
      <b-row>
        <b-col md="6">
          <h3 class="AboutUs-fond__title">Nuestra trayectoria</h3>
          <span class="AboutUs-fond__mind"
            >CECITEL tiene más de 20 años de experiencia en el campo educativo,
            formando técnicos especializados en Telemarketing, Atención al
            Cliente, Supervisores para Call Center y Reparación de
            Celulares.</span
          >
          <p class="AboutUs-fond__paragraph">
            Como pioneros en estas actividades que marcaron el crecimiento
            económico de las telecomunicaciones en nuestro país, nos sentimos
            satisfechos de haber aportado una importante cuota de jóvenes
            calificados al mercado laboral.
          </p>
        </b-col>
        <b-col md="6">
          <img
            :src="require('@/assets/img/about/nuestra_trayectoria.png')"
            alt="nuestra trayectoria"
            class="AboutUs-fond__img"
          />
        </b-col>
      </b-row>
      <b-row>
        <b-col md="6">
          <img
            :src="require('@/assets/img/about/valores.png')"
            alt="valores"
            class="AboutUs-fond__img"
          />
        </b-col>
        <b-col md="6">
          <div class="text-md-right">
            <h3 class="AboutUs-fond__title">Valores que nos definen</h3>
            <p class="AboutUs-fond__paragraph">
              Cuando compartimos experiencias e interactuamos contigo,
              conectamos tus necesidades con nuestra vocación de enseñanza, para
              juntos llegar a destinos nuevos con oportunidades para todos en
              los diferentes sectores en los que buscas desarrollarte.
            </p>
          </div>
        </b-col>
      </b-row>
    </b-container>
    <div class="AboutUs-fond">
      <b-container>
        <p class="AboutUs-fond__text">
          El enfoque por competencias laborales desarrolla el SABER SER, SABER
          HACER, SABER CONOCER Y SABER ESTAR, impregnado de valores éticos que
          aseguran un elevado estándar de calidad de trabajo en las
          organizaciones a las que pertenecen.
        </p>
      </b-container>
    </div>
    <b-container>
      <b-row>
        <b-col md="6">
          <h3 class="AboutUs-fond__title">Evolución y adaptación</h3>
          <p class="AboutUs-fond__paragraph">
            El Teletrabajo se ha convertido en una estrategia efectiva para
            mantener operativas a las organizaciones de todos los rubros. <br />
            CECITEL evoluciona brindando herramientas para desarrollar nuevos
            aprendizajes desde la comodidad de tu hogar y potenciar tus
            habilidades personales y profesionales.
          </p>
        </b-col>
        <b-col md="6">
          <img
            :src="require('@/assets/img/about/evolucion.png')"
            alt="evolucion y adaptacion"
            class="AboutUs-fond__img"
          />
        </b-col>
      </b-row>
      <b-row>
        <b-col md="6">
          <img
            :src="require('@/assets/img/about/cursos_para_todos.png')"
            alt="Cursos para todos"
            class="AboutUs-fond__img"
          />
        </b-col>
        <b-col md="6">
          <div class="text-md-right">
            <h3 class="AboutUs-fond__title">Cursos para todos</h3>
            <p class="AboutUs-fond__paragraph">
              Nos dirigimos a los emprendedores, jubilados, personas con
              discapacidad motora y visual, dependientes e independientes, que
              busquen capacitación especializada para potenciar sus recursos
              personales y sus oportunidades de negocios.
            </p>
            <span class="AboutUs-fond__mind">
              Ahora nos convertimos en una plataforma tecnológica que brinda
              cursos semipresenciales, talleres vivenciales, cursos online,
              dirigidos a las personas que apuesten por su crecimiento y
              desarrollo en adquirir herramientas tecnológicas y habilidades
              directivas.
            </span>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'

export default {
  name: 'AboutUs',
  components: { BannerTop },
  data() {
    return {
      image: require('@/assets/img/banner/about.jpg'),
    }
  },
}
</script>

<style lang="css" scoped>
.AboutUs-fond {
  background-image: url('@/assets/img/about/conocenos.svg');
  background-size: cover;
  min-height: 550px;
}

.AboutUs-fond__text {
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 45px;
  text-align: center;
  color: #568ae9;
  width: 100%;
  height: 100%;
}

.AboutUs-fond__title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
  color: #568ae9;
}

.AboutUs-fond__paragraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
  color: #000;
}
.AboutUs-fond__mind {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
  color: #568ae9;
}
</style>
