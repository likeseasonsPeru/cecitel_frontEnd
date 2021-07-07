<template>
  <div class="Pay">
    <b-container>
      <b-row>
        <b-col md="5" class="Pay__Section">
          <div class="Pay__Section-pay">
            <h1 class="Pay__Section-title">Confirma tu compra</h1>
            <div class="d-flex">
              <b-button class="Pay__Section-pay-button mr-1" size="lg"
                >Tarjeta</b-button
              >
              <b-button class="Pay__Section-pay-button ml-1" size="lg"
                >Efectivo</b-button
              >
            </div>
            <div class="Pay__Section-pay-name my-4">
              <span>Tipo de tarjeta</span>
            </div>
            <div class="d-flex">
              <img
                :src="require('@/assets/img/pay/visa.png')"
                alt=""
                class="img-fluid img mx-2"
              />
              <img
                :src="require('@/assets/img/pay/mcard.png')"
                alt=""
                class="img-fluid img mx-2"
              />
            </div>
            <b-form>
              <div class="mt-4">
                <label class="Pay__Section-pay-name" for=""
                  >Nombre de la tarjeta</label
                ><br />
                <input class="Pay__Section-pay-input" type="text" />
              </div>
              <label class="Pay__Section-pay-name mt-4" for=""
                >Número de tarjeta</label
              ><br />
              <input class="Pay__Section-pay-input" type="text" />
              <b-row>
                <b-col md="8">
                  <label class="Pay__Section-pay-name mt-4" for=""
                    >Fecha de expiración</label
                  ><br />
                  <input class="Pay__Section-pay-input" type="text" />
                </b-col>
                <b-col md="4">
                  <label class="Pay__Section-pay-name mt-4" for="">CVV</label
                  ><br />
                  <input class="Pay__Section-pay-input" type="text" />
                </b-col>
              </b-row>

              <b-button
                type="submit"
                class="Pay__Section-pay-submit my-5"
                pill
                block
                >Comprar</b-button
              >
            </b-form>
          </div>
        </b-col>
        <b-col md="7">
          <div class="Pay__Section-shop">
            <h1 class="Pay__Section-shop-name">Carrito</h1>
            <span class="Pay__Section-shop-items"
              >Tienes 2 Ítems en tu carrito</span
            >
            <div>
              <div v-for="item in data" :key="item.title">
                <PayCourseCard :item="item" />
              </div>
            </div>
          </div>
          <div class="Pay__Section-total my-4">
            <p>Total a pagar:</p>
            <span>s/ 130.00</span>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import PayCourseCard from '../cards/PayCourseCard.vue'
export default {
  name: 'Pay',
  components: { PayCourseCard },
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
    }
  },
}
</script>

<style scoped>
.img {
  width: 63px;
  height: 50px;
  padding: 5px;
  border: 1px solid #fff;
  border-radius: 5px;
}
.Pay__Section {
  /* background-color: linear-gradient(135deg, #4a90e2 0%, #4275d2 100%); */
  background-color: #4a90e2;
}
.Pay__Section-pay {
  padding: 20px 40px;
}
.Pay__Section-title {
  font-weight: bold;
  font-size: 30px;
  line-height: 45px;
  color: #fff;
}
.Pay__Section-shop-name {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
}
.Pay__Section-shop-items {
  font-weight: 300;
  font-size: 24px;
  line-height: 36px;
}
.Pay__Section-shop {
  border-bottom: 1px solid #a1a1a1;
}
.Pay__Section-total {
  display: flex;
  justify-content: space-between;
  font-weight: bold;
  font-size: 30px;
  line-height: 45px;
  color: #222;
}
.Pay__Section-pay-button {
  width: 50%;
  background: #fff;
  border: none;
  border-radius: 20px;
  font-weight: bold;
  font-size: 24px;
  line-height: 36px;
  color: #568ae9;
}

/* form */
.Pay__Section-pay-name {
  font-weight: bold;
  font-size: 18px;
  line-height: 27px;
  color: #fff;
}
.Pay__Section-pay-input {
  border: none;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 15px;
  width: 100%;
  min-height: 50px;
  padding: 0 10px;
}
.Pay__Section-pay-submit {
  background: #fff;
  border: none;
  border-radius: 33.5px;
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  color: #467ad9;
}
</style>
