<template>
  <div class="TeleSalesCorp">
    <BannerTop :image="image" />
    <b-container>
      <b-row>
        <b-col>
          <h3 class="TeleSalesCorp-title">Televentas</h3>
          <h6>Curso personalizado</h6>
          <p class="TeleSalesCorp-paragraph">
            Creado para un grupo determinado de integrantes, cumpliendo con
            todos nuestros estándares. Nos reinventamos para ustedes y les
            brindamos un programa 100% ONLINE con clases totalmente en vivo
            pensando en un momento de aprendizaje e integración con tus
            compañeros. Contrary to popular belief, Lorem Ipsum is not simply
            random text. It has roots in a piece of classical Latin literature
            from 45 BC, making it over 2000 years old. Richard McClintock, a
            Latin professor at Hampden-Sydney College in Virginia. Looked up one
            of the more obscure Latin words, consectetur, from a Lorem Ipsum
            passage, and going through the cites of the word in classical
            literature, discovered the undoubtable source. Lorem Ipsum comes
            from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum.
          </p>
          <h6>Objetivo del curso</h6>
          <p class="TeleSalesCorp-paragraph">
            Contrary to popular belief, Lorem Ipsum is not simply random text.
            It has roots in a piece of classical Latin literature from 45 BC,
            making it over 2000 years old. Richard McClintock, a Latin professor
            at Hampden-Sydney College in Virginia. Looked up one of the more
            obscure Latin words, consectetur, from a Lorem Ipsum passage, and
            going through the cites of the word in classical literature,
            discovered the undoubtable source. Lorem Ipsum comes from sections
            1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum.
          </p>
        </b-col>
        <b-col>
          <ContactForm />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'
import ContactForm from '~/components/partials/forms/ContactForm.vue'
export default {
  name: 'TeleSalesCorp',
  components: { BannerTop, ContactForm },
  data() {
    return {
      image: require('@/assets/img/banner/televentas.jpg'),
    }
  },
}
</script>
