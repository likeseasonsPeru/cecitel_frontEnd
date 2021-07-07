<template>
  <div class="ContactForm">
    <div>
      <h3>Inscribíbete aquí</h3>
    </div>
    <div>
      <b-form v-if="show" @submit.prevent="onSubmit">
        <b-form-group
          id="input-group-2"
          label="Nombres y Apellidos"
          label-for="input-2"
        >
          <b-form-input
            id="input-2"
            v-model="form.nameCompleted"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group
          id="phone-group"
          label="Teléfono"
          label-for="phone-input"
          label-class="label-form"
        >
          <b-form-input
            id="phone-input"
            v-model="form.phone"
            v-mask="'9########'"
            type="tel"
            name="phone-input"
          ></b-form-input>
        </b-form-group>
        <b-form-group id="input-group-1" label="Correo" label-for="input-1">
          <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            required
          ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-4" v-slot="{ ariaDescribedby }">
          <b-form-checkbox-group
            id="checkboxes-4"
            v-model="form.checked"
            :aria-describedby="ariaDescribedby"
          >
            <b-form-checkbox value="me"
              >Deseas recibir información de los cursos y otros servicios que
              brinda Cecitel</b-form-checkbox
            >
            <b-form-checkbox value="that"
              >He leído y acepto la pólitica de privacidad</b-form-checkbox
            >
          </b-form-checkbox-group>
        </b-form-group>
        <div>
          <div>
            <span>TOTAL</span>
            <span>s/ 50.00</span>
          </div>
          <b-button pill block type="submit" href="/webinars/pagar"
            >Pagar</b-button
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
      </b-form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'InscriptionForm',
  data() {
    return {
      form: {
        email: '',
        nameCompleted: '',
        form: null,
        checked: [],
      },
      show: true,
    }
  },
  methods: {
    onSubmit() {
      alert(JSON.stringify(this.form))
    },
  },
}
</script>

<style lang="css" scoped>
.ContactForm {
  background-color: #fafafa;
}
</style>
