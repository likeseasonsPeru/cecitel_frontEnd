<template>
  <div class="ShoppingCart">
    <b-container class="section">
      <b-row>
        <b-col md="8" class="">
          <div class="d-flex pb-4 ShoppingCart__Cart">
            <img
              :src="require('~/components/svg/icons/chevron-left.svg')"
              alt="icon left"
            />
            <span class="ml-3">Seguir comprando</span>
          </div>
          <div>
            <h3 class="ShoppingCart__Cart-title">Carrito</h3>
            <span class="ShoppingCart__Cart-text"
              >Tienes 3 Ítems en tu carrito</span
            >
            <div v-for="item in data" :key="item.title">
              <PayCourseCard :item="item" />
            </div>
          </div>
        </b-col>
        <b-col md="4">
          <b-card class="ShoppingCart__total">
            <h4 class="ShoppingCart__total-title">Resumen de Compra</h4>
            <div class="ShoppingCart__total-item my-3">
              <span>En el carrito:</span>
              <span>s/ 0.00</span>
            </div>
            <div class="ShoppingCart__total-item my-3">
              <span>Descuentos:</span>
              <span>s/ 0.00</span>
            </div>
            <div class="ShoppingCart__total-item my-3">
              <span>Total:</span>
              <span>s/ 0.00</span>
            </div>
            <b-button pill block>Pagar</b-button>
            <p>
              Recuerda que los cursos enlatados tienen un tiempo limite de 6
              meses de visualización.
            </p>
          </b-card>
        </b-col>
      </b-row>
      <div class="ShoppingCart__recommended">
        <h3 class="ShoppingCart__recommended-title">Recomendados</h3>
        <div class="ShoppingCart__recommended-cart">
          <div v-for="item in data1" :key="item.title">
            <CourseCard :item="item" />
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import CourseCard from '~/components/partials/cards/CourseCard.vue'
import PayCourseCard from '~/components/partials/cards/PayCourseCard.vue'
export default {
  name: 'ShoppingCart',
  components: { PayCourseCard, CourseCard },
  data() {
    return {
      data: [
        {
          image: require('@/assets/img/courses/curso1.png'),
          title: 'Taller de adaptación a procesos de cambios',
          teacher: 'Profesor a cargo',
          price: 's/ 50.00',
        },
        {
          image: require('@/assets/img/courses/curso2.png'),
          title: 'Nombre del curso',
          teacher: 'Profesor a cargo',
          price: 's/ 50.00',
        },
        {
          image: require('@/assets/img/courses/curso1.png'),
          title: 'Excel Avanzado',
          teacher: 'Profesor a cargo',
          price: 's/ 30.00',
        },
      ],
      data1: [
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
      ],
    }
  },
}
</script>

<style>
.ShoppingCart__Cart {
  border-bottom: 1px solid #9d9d9d;
}

/* cart */
.ShoppingCart__Cart-title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
}
.ShoppingCart__Cart-text {
  font-weight: normal;
  font-size: 24px;
  line-height: 36px;
}

/* recommended */
.ShoppingCart__recommended-title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
}
.ShoppingCart__recommended-cart {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

/* total */
.ShoppingCart__total {
  border: none;
  background: #fafafa;
  border-radius: 20px;
}
.ShoppingCart__total-title {
  text-align: center;
  font-weight: bold;
  font-size: 30px;
  line-height: 45px;
  color: #568ae9;
}
.ShoppingCart__total-item {
  display: flex;
  justify-content: space-between;
}
</style>
