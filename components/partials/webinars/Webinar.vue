<template>
  <div class="Webinar">
    <BannerTop :image="image" />
    <b-container>
      <div>
        <div>
          <h3 class="Webinar-title">Webinars</h3>
          <p class="Webinar-paragraph">
            La tecnología nos permite estar cerca de Ti, con novedades y
            tendencias para enriquecer tus conocimientos en los diferentes
            aspectos de tu vida personal, social y laboral. <br />
            Desde donde estés accede a nuestro catálogo de webinars, elije ahora
            y comparte una experiencia valiosa para Ti.
          </p>
        </div>
        <div>
          <div v-for="(item, index) in dataWebinars" :key="index">
            <WebinarCard :item="item" />
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'
import WebinarCard from '~/components/partials/cards/WebinarCard.vue'
export default {
  name: 'Webinar',
  components: { BannerTop, WebinarCard },
  data() {
    return {
      image: require('@/assets/img/banner/webinars.jpg'),
      dataWebinars: [
        {
          title: 'Coaching con Inteligencia Emocional',
          paragraph:
            "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden.",
          date: '15 de Octubre',
          time: '07:00pm',
          price: 'Gratuito',
        },
        {
          title: 'Taller de adaptación a procesos de cambio',
          paragraph:
            "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden.",
          date: '15 de Octubre',
          time: '07:00pm',
          price: 's/ 50.00',
        },
      ],
    }
  },
}
</script>

<style>
.Webinar-title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
  color: #4a90e2;
}
.Webinar-paragraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
  color: #000;
}
</style>
