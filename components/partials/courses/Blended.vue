<template>
  <div class="Blended">
    <b-container>
      <div>
        <b-card img-alt="Card image" img-right class="Blended__card">
          <div class="Blended__card-data d-flex">
            <div class="Blended__card-data-content">
              <h1 class="Blended__card-dataTitle">Aprende con nosotros</h1>
              <b-card-text class="Blended__card-dataParagraph">
                Obten un 15% de descuento en tus clases online <br />
                solo registrandote
              </b-card-text>
              <b-button pill class="Blended__card-dataButton">Ver más</b-button>
            </div>
            <div>
              <img
                :src="require('@/assets/img/courses/blended.svg')"
                alt="Semipresenciales Course"
                class="img-fluid"
              />
            </div>
          </div>
        </b-card>
      </div>
      <div>
        <b-row>
          <b-col md="3">
            <FilterCourses />
          </b-col>
          <b-col md="9">
            <div class="ml-2">
              <h1 class="Blended__head">Semipresenciales</h1>
              <p class="Blended__paragraph">
                A distancia, pero bajo la dirección de un experto docente, con
                quien puedes interactuar, hacer preguntas y participar
                activamente en los trabajos grupales, dentro de la plataforma
                virtual.
              </p>
            </div>
            <div class="Blended__cards">
              <div v-for="item in data" :key="item.title">
                <CourseCard :item="item" />
              </div>
            </div>
          </b-col>
        </b-row>
      </div>
    </b-container>
  </div>
</template>

<script>
import CourseCard from '~/components/partials/cards/CourseCard.vue'
import FilterCourses from '~/components/partials/courses/FilterCourses.vue'
export default {
  name: 'Blended',
  components: { CourseCard, FilterCourses },
  data() {
    return {
      data: [
        {
          image: require('@/assets/img/courses/cursocomunicacion.png'),
          title: 'Comunicación efectiva en redes sociales',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
        {
          image: require('@/assets/img/courses/cursoexcel.png'),
          title: 'Curso de Excel básico, intermedio y avanzado',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
        {
          image: require('@/assets/img/courses/cursoredes.png'),
          title: 'Comunicación efectiva en redes sociales',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
        {
          image: require('@/assets/img/courses/cursoventas.png'),
          title: 'Curso de televentas efectivas',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
        {
          image: require('@/assets/img/courses/cursoexcel2.png'),
          title: 'Curso de Excel empresarial avanzado',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
        {
          image: require('@/assets/img/courses/cursoredes2.png'),
          title: 'Comunicación efectiva en redes sociales',
          paragraph:
            'It was popularised in the with the release of Letraset sheets containing and more recently…',
        },
      ],
    }
  },
}
</script>

<style>
.Blended__cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-row-gap: wrap;
}
.Blended {
  padding: 60px 0;
}
.Blended__card {
  color: #fff;
  background-color: #9c73d4;
  border: none;
  border-radius: 20px;
  max-height: 351px;
}
.Blended__head {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
  color: #4a90e2;
  margin-top: 50px;
}
.Blended__paragraph {
  font-size: 18px;
  line-height: 28px;
}
.Blended__card-data {
  display: flex;
  justify-content: space-between;
}
.Blended__card-data-content {
  margin-left: 60px;
}
.Blended__card-dataTitle {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
}
.Blended__card-dataParagraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
}
.Blended__card-dataButton {
  color: #9c73d4;
  background: #fff;
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  padding: 18px 70px;
}
</style>
