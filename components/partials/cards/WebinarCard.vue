<template>
  <div class="WebinarCard my-5">
    <b-card>
      <h4 class="WebinarCard-title">{{ item.title }}</h4>
      <b-card-text class="WebinarCard-paragraph">
        {{ item.paragraph }}
      </b-card-text>
      <div class="WebinarCard-terms d-flex">
        <div>
          <img
            :src="require('@/assets/img/icons/watch.svg')"
            alt="Watch-icon"
          />
          <span class="mb-1">{{ item.date }}</span>
          <br />
          <img
            :src="require('@/assets/img/icons/calendar.svg')"
            alt="Calendar-icon"
          />
          <span class="mb-1">{{ item.time }}</span>
        </div>
        <div>
          <span>{{ item.price }}</span> <br />
          <b-button pill>Incríbete</b-button>
        </div>
      </div>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'WebinarCard',
  props: {
    item: {
      type: Object,
      default() {
        return {
          title: 'Coaching con Inteligencia Emocional',
          paragraph:
            "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden.",
          date: '15 de Octubre',
          time: '07:00pm',
          price: 'Gratuito',
        }
      },
    },
  },
}
</script>

<style>
.WebinarCard {
  border-radius: 20px;
}
.card {
  border: none;
  background-color: #fafafa;
  border-radius: 20px;
  padding: 26px 42px 22px;
}
.WebinarCard-title {
  font-weight: bold;
  font-size: 25px;
  line-height: 37px;
}
.WebinarCard-paragraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
}
.WebinarCard-terms {
  justify-content: space-between;
}
</style>
