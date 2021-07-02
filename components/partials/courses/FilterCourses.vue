<template>
  <div class="FilterCourses">
    <div>
      <b-form-group v-slot="{ ariaDescribedby }">
        <span class="FilterCourses__type">Categorías</span>
        <b-form-checkbox-group
          id="checkbox-group-1"
          v-model="selected"
          :aria-describedby="ariaDescribedby"
          name="flavour-1"
          stacked
        >
          <b-form-checkbox value="semipresencial"
            >Semipresencial</b-form-checkbox
          >
          <b-form-checkbox value="online">Online</b-form-checkbox>
        </b-form-checkbox-group>
      </b-form-group>
    </div>
    <div>
      <b-form-group v-slot="{ ariaDescribedby }" class="mt-5">
        <span class="FilterCourses__type">Duración</span>
        <b-form-checkbox-group
          id="checkbox-group-2"
          v-model="selected"
          :aria-describedby="ariaDescribedby"
          name="flavour-2"
          stacked
        >
          <b-form-checkbox value="32">32 horas</b-form-checkbox>
          <b-form-checkbox value="16">16 horas</b-form-checkbox>
          <b-form-checkbox value="8">8 horas</b-form-checkbox>
        </b-form-checkbox-group>
      </b-form-group>
    </div>
    <div>
      <b-form-group v-slot="{ ariaDescribedby }" class="mt-5">
        <span class="FilterCourses__type">Dificultad</span>
        <b-form-checkbox-group
          id="checkbox-group-3"
          v-model="selected"
          :aria-describedby="ariaDescribedby"
          name="flavour-3"
          stacked
        >
          <b-form-checkbox value="basico">Básico</b-form-checkbox>
          <b-form-checkbox value="intermedio">Intermedio</b-form-checkbox>
          <b-form-checkbox value="avanzado">Avanzado</b-form-checkbox>
        </b-form-checkbox-group>
      </b-form-group>
    </div>
    <div>
      <b-form-group v-slot="{ ariaDescribedby }" class="mt-5">
        <span class="FilterCourses__type">Certificado</span>
        <b-form-checkbox-group
          id="checkbox-group-4"
          v-model="selected"
          :aria-describedby="ariaDescribedby"
          name="flavour-4"
          stacked
        >
          <b-form-checkbox value="gratuito">Gratuito</b-form-checkbox>
          <b-form-checkbox value="pago"
            >De Pago</b-form-checkbox
          ></b-form-checkbox-group
        >
      </b-form-group>
    </div>
    {{ selected }}
  </div>
</template>

<script>
export default {
  name: 'FilterCourses',
  data() {
    return {
      selected: [], // Must be an array reference!
      optionsCategories: [
        { text: 'Semipresencial', value: 'semipresencial' },
        { text: 'Online', value: 'online' },
      ],
      optionsDuring: [
        { text: '32 horas', value: '32' },
        { text: '16 horas', value: '16' },
        { text: '8 horas', value: '8' },
      ],
      optionsDificult: [
        { text: 'Básico', value: 'basico' },
        { text: 'Intermedio', value: 'intermedio' },
        { text: 'Avanzado', value: 'avanzado' },
      ],
      optionsCertificate: [
        { text: 'Gratuito', value: 'gratuito' },
        { text: 'De pago', value: 'pago' },
      ],
    }
  },
}
</script>

<style lang="css" scoped>
.custom-control {
  font-size: 18px;
  margin-top: 23px;
}
.FilterCourses {
  background-color: #fafafa;
  border-radius: 20px;
  margin-top: 97px;
  padding: 38px 41px;
}
.FilterCourses__type {
  font-weight: bold;
  font-size: 21px;
  line-height: 31px;
  color: #000;
}
.FilterCourses__item {
  font-size: 21px;
  line-height: 35px;
}
</style>
