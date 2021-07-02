<template>
  <div class="CoachingCorp">
    <BannerTop :image="image" />
    <b-container>
      <b-row>
        <b-col>
          <h3 class="CoachingCorp-title">Coaching</h3>
          <p class="CoachingCorp-paragraph">
            El coaching como estrategia potente, para lograr el
            autodescubrimiento de tus talentos y sueños, ahora al alcance de tus
            manos. <br />
            Las personas fácilmente ayudamos a otras a encaminarse, orientarse y
            hasta comprometerse con lo que quieren en la vida; sin embargo, es
            difícil autoanalizarnos y darnos cuenta qué potencialidades tenemos
            guardadas en lo más profundo de nuestro Ser. <br />
            Con un paquete de sesiones de coaching lograrás esto y mucho más,
            para conseguir bienestar en tu vida personal y laboral. <br />
            Reserva tu cita y te confirmaremos la primera sesión.
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
  name: 'CoachingCorp',
  components: { BannerTop, ContactForm },
  data() {
    return {
      image: require('@/assets/img/banner/coaching.jpg'),
    }
  },
}
</script>
