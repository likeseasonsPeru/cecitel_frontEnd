<template>
  <div class="ContactForm">
    <div>
      <h3>Escríbenos</h3>
      <span>Y recibe atención personalizada</span>
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

        <b-form-group
          id="input-group-3"
          label="¿ A qué hora puedo llamarte ?"
          label-for="input-3"
        >
          <b-form-select
            id="input-3"
            v-model="form.food"
            :options="foods"
            required
          ></b-form-select>
        </b-form-group>
        <b-form-group
          id="commentary-group"
          label="Mensaje"
          label-for="unid-input"
          label-class="label-form"
        >
          <b-form-textarea
            id="commentary-input"
            v-model="form.commentary"
            rows="3"
            name="commentary-input"
          ></b-form-textarea>
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

        <b-button class="text-center" type="submit" variant="primary"
          >Enviar</b-button
        >
      </b-form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactForm',
  data() {
    return {
      form: {
        email: '',
        nameCompleted: '',
        form: null,
        food: null,
        checked: [],
        commentary: '',
      },
      foods: [
        { text: 'Selecciona un horario', value: null },
        '9:00 am a 10:00 am',
        '10:00 am a 11:00 am',
        '11:00 am a 12:00 pm',
        '12:00 pm a 1:00 pm',
        '1:00 pm a 2:00 pm',
        '2:00 pm a 3:00 pm',
      ],
      show: true,
    }
  },
  methods: {
    onSubmit(event) {
      event.preventDefault()
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
