<template>
  <div class="Inscription">
    <BannerTop :image="image" />
    <b-container class="section">
      <b-row>
        <b-col md="6">
          <div class="Incription__data">
            <h1>Taller de adaptación a procesos de cambio</h1>
            <span>s/ 50.00</span>
            <div class="d-flex">
              <img
                :src="require('@/assets/img/courses/teach-course.jpg')"
                alt=""
              />
              <span class="ml-3"
                >Nombres y Apellidos <br />
                Cargos</span
              >
            </div>
            <p>
              Creado para un grupo determinado de integrantes, cumpliendo con
              todos nuestros estándares. Nos reinventamos para ustedes y les
              brindamos un programa 100% ONLINE con clases totalmente en vivo
              pensando en un momento de aprendizaje e integración con tus
              compañeros.
            </p>
            <h4>OBJETIVO DEL TALLER</h4>
            <p>
              Contrary to popular belief, Lorem Ipsum is not simply random text.
              It has roots in a piece of classical Latin literature from 45 BC,
              making it over 2000 years old. Richard McClintock, a Latin
              professor at Hampden-Sydney College in Virginia. <br />
              Looked up one of the more obscure Latin words, consectetur, from a
              Lorem Ipsum passage, and going through the cites of the word in
              classical literature, discovered the undoubtable source. Lorem
              Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus
              Bonorum et Malorum.
            </p>
            <b-card>
              <div class="d-flex">
                <div class="d-flex">
                  <img :src="require('@/assets/img/icons/time.png')" alt="" />
                  <span>Duracion</span>
                </div>
                <div>
                  <span>2 Horas</span>
                </div>
              </div>
              <div class="d-flex">
                <div class="d-flex">
                  <img
                    :src="require('@/assets/img/icons/calendar.svg')"
                    alt=""
                  />
                  <span>Fecha</span>
                </div>
                <div>
                  <span>15 de Octubre</span>
                </div>
              </div>
              <div class="d-flex">
                <div class="d-flex">
                  <img :src="require('@/assets/img/icons/cupos.png')" alt="" />
                  <span>Cupos</span>
                </div>
                <div>
                  <span>20</span>
                </div>
              </div>
            </b-card>
          </div>
        </b-col>
        <b-col md="6">
          <InscriptionForm />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'
import InscriptionForm from '~/components/partials/forms/IncriptionForm.vue'
export default {
  name: 'Inscription',
  components: { BannerTop, InscriptionForm },
  data() {
    return {
      image: require('@/assets/img/banner/taller.jpg'),
    }
  },
}
</script>

<style>
.Inscription {
  font-size: 16px;
}
</style>
