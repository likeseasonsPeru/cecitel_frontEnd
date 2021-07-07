<template>
  <div class="Course">
    <BannerTop :image="image" />
    <b-container class="section">
      <b-row>
        <b-col md="9">
          <div>
            <img
              :src="require('@/assets/img/courses/icons/vendido.png')"
              alt="Más vendido"
              class="my-5"
            />
            <h1>
              Comunicación efectiva en <br />
              redes sociales
            </h1>
            <b-tabs content-class="mt-3" justified>
              <b-tab title="Información" active>
                <p>
                  Hoy, más que nunca, es necesario potenciar nuestras
                  habilidades de comunicación verbal y no verbal, para
                  desarrollarnos en el competitivo mercado laboral que tenemos y
                  aprovechar las oportunidades que nos brinda el avance
                  tecnológico de la comunicación digital.
                </p>
                <h4>Materiales</h4>
                <div class="d-flex">
                  <img
                    :src="require('@/assets/img/courses/icons/materiales.png')"
                    alt="materiales"
                  />
                  <p>
                    Lorem Ipsum has been the industry's standard dummy text ever
                    since.
                  </p>
                </div>
                <h4>Objetivos</h4>
                <p>
                  Lorem Ipsum has been the industry's standard dummy text ever
                  since the 1500s, when an unknown printer took a galley of type
                  and scrambled it to make a type specimen book. It has survived
                  not only five centuries, but also
                </p>
                <h4>Duración</h4>
                <div class="d-flex">
                  <img
                    :src="require('@/assets/img/courses/icons/duracion.png')"
                    alt="duracion"
                    style="height: 52px"
                  />
                  <p>
                    30 horas <br />
                    2 meses <br />
                    2 veces por semana
                  </p>
                </div>
                <p>
                  It is a long established fact that a reader will be distracted
                  by the readable content of a page when looking at its layout.
                </p>
                <h4>Nivel de dificultad</h4>
                <div class="d-flex">
                  <img
                    :src="require('@/assets/img/courses/icons/tiempo.png')"
                    alt="tiempo"
                  />
                  <p>6 meses</p>
                </div>
                <p>
                  La visualización del curso estará disponible en la plataforma
                  por el transcurso de 6 meses desde el día en el que sea
                  adquirido, en este tiempo usted podrá aceder a los videos,
                  archivos y otros contenidos que el curso ofrece.
                </p>
              </b-tab>
              <b-tab title="Unidades">
                <div class="Course__unids">
                  <h3 class="Course__unids-title">UD1</h3>
                  <div class="Course__unids-body">
                    <p>Herramientas de manejo de redes digitales</p>
                    <span
                      ><img
                        :src="require('@/assets/img/courses/icons/clock.svg')"
                        alt=""
                      />
                      15 horas</span
                    >
                  </div>
                  <h3 class="Course__unids-title">UD2</h3>
                  <div class="Course__unids-body">
                    <p>Comunicación audiovisual efectiva</p>
                    <span
                      ><img
                        :src="require('@/assets/img/courses/icons/clock.svg')"
                        alt=""
                      />
                      15 horas</span
                    >
                  </div>
                </div>
              </b-tab>
              <b-tab title="Temarios">
                <div class="Course__data">
                  <ul class="Course__data-items">
                    <li>Importancia de las plataformas digitales.</li>
                    <li>
                      Gestión de plataformas como: Facebook, Instagram, LinkedIn
                      y otras.
                    </li>
                    <li>Comunicación audiovisual.</li>
                    <li>Storytelling (concepto-usos)</li>
                    <li>
                      Herramientas de comunicación efectiva no verbal: Tono de
                      voz adecuado Contacto visual
                    </li>
                    <li>
                      Herramientas telemáticas sincrónicas y asincrónicas para
                      la comunicación. Comunicación simultánea bidireccional:
                      Chat y Videoconferencia
                    </li>
                    <li>
                      Tipos de conferencias de acuerdo a los recursos
                      utilizados.
                    </li>
                    <li>
                      Comunicación paraverbal: volumen, entonación, velocidad
                    </li>
                    <li>Expresión oral y manejo de escenario.</li>
                    <li>Capacidad de persuasión</li>
                    <li>Manejo de tiempo</li>
                    <li>Storytelling (estratégico)</li>
                  </ul>
                </div>
              </b-tab>
              <b-tab title="Profesor">
                <div class="Course__teacher">
                  <div class="d-flex">
                    <img
                      :src="require('@/assets/img/courses/teach-course.jpg')"
                      alt=""
                    />
                    <span class="Course__teacher-name ml-3"
                      >Nombres y Apellidos <br />
                      Cargos</span
                    >
                  </div>
                  <p class="Course__teacher-paragraph">
                    It is a long established fact that a reader will be
                    distracted by the readable content of a page when looking at
                    its layout. The point of using Lorem Ipsum is that it has a
                    more-or-less normal distribution of letters, as opposed to
                    using 'Content here, content here', making it look like
                    readable English. Many desktop publishing packages and web
                    page editors now use Lorem Ipsum as their default model
                    text, and a search for 'lorem ipsum' will uncover many web
                    sites still in their infancy. Various versions have evolved
                    over the years, sometimes by accident, sometimes on purpose
                    (injected humour and the like).
                  </p>
                </div>
              </b-tab>
            </b-tabs>
          </div>
        </b-col>
        <b-col md="3">
          <b-card
            :img-src="require('@/assets/img/courses/cursocomunicacion.png')"
            img-alt="Image"
            img-top
            tag="article"
            class="CourseCard mx-3 mb-4 text-center"
          >
            <span class="CourseCard__price">s/ 0.00</span>
            <div>
              <b-button pill block class="CourseCard__button my-3"
                >Comprar</b-button
              >
              <span class="CourseCard__free">Quedan disponibles 3 cupos</span>
              <div class="CourseCard__icons my-3">
                <div>
                  <img
                    :src="require('@/assets/img/courses/icons/shop.svg')"
                    alt=""
                  />
                  <br />
                  <span class="CourseCard__icons-name">Carrito</span>
                </div>
                <div>
                  <img
                    :src="require('@/assets/img/courses/icons/heart.svg')"
                    alt=""
                  />
                  <br />
                  <span class="CourseCard__icons-name">Favoritos</span>
                </div>
                <div>
                  <img
                    :src="require('@/assets/img/courses/icons/share.svg')"
                    alt=""
                  />
                  <br />
                  <span class="CourseCard__icons-name">Compartir</span>
                </div>
              </div>
            </div>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'
export default {
  name: 'Course',
  components: { BannerTop },
  data() {
    return {
      image: require('@/assets/img/banner/semipresencial.jpg'),
    }
  },
}
</script>

<style scoped>
.CourseCard {
  border: none;
  background: #fafafa;
  box-shadow: 0 3px 11px rgba(173, 173, 173, 0.5);
  border-radius: 20px;
  margin-top: 150px;
}
.CourseCard__price {
  float: right;
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
  color: #4275d2;
}
.CourseCard__button {
  border: none;
  background: linear-gradient(270deg, #7bbbef 2.04%, #4275d2 97.45%);
  border-radius: 23px;
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  color: #fff;
}
.CourseCard__free {
  font-weight: normal;
  font-size: 12px;
  line-height: 18px;
  color: #000;
}
.CourseCard__icons {
  display: flex;
  justify-content: space-between;
}
.CourseCard__icons-name {
  font-weight: 500;
  font-size: 12px;
  line-height: 18px;
  color: #7bbbef;
}
.Course__teacher-name {
  display: flex;
  align-items: center;
  color: #227a5d;
  font-weight: bold;
  font-size: 25px;
  line-height: 37px;
}
.Course__teacher-paragraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
}
.Course__data-items {
  font-weight: bold;
  font-size: 21px;
  line-height: 49px;
  list-style: square;
}
.Course__unids-title {
  font-weight: bold;
  font-size: 25px;
  line-height: 37px;
  color: #227a5d;
}
.Course__unids-body {
  display: flex;
  justify-content: space-between;
  background: #fafafa;
  border-radius: 20px;
  padding: 20px 20px 8px;
  font-size: 21px;
}
</style>
