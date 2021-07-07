<template>
  <div class="PayCourseCard my-3">
    <b-card
      :img-src="item.image"
      img-alt="Card image"
      img-left
      class="PayCourseCard__card"
    >
      <b-row class="PayCourseCard__card-file">
        <b-col md="6">
          <span class="PayCourseCard__card-name">
            {{ item.title }}
          </span>
          <br />
          <span class="PayCourseCard__card-teacher">{{ item.teacher }}</span>
        </b-col>
        <b-col md="4" class="PayCourseCard__card-box">
          <div class="PayCourseCard__card-price">
            <span>{{ item.price }}</span>
          </div>
        </b-col>
        <b-col md="2" class="PayCourseCard__card-box">
          <div>
            <img
              :src="require('@/assets/img/courses/icons/trash.svg')"
              alt="trash"
            />
          </div>
        </b-col>
      </b-row>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'PayCourseCard',
  props: {
    item: {
      type: Object,
      default() {
        return {
          image: require('@/assets/img/courses/icons/trash.svg'),
          title: 'Taller de adaptación a procesos de cambios',
          teacher: 'Profesor a cargo',
          price: 's/ 50.00',
        }
      },
    },
  },
}
</script>

<style>
.card {
  border: none;
  border-radius: 20px;
}
.card-img-left {
  padding: 20px;
  max-width: 100%;
  height: auto;
}
.PayCourseCard__card-file {
  height: 100%;
}
.PayCourseCard__card {
  background-color: #fafafa;
}
.PayCourseCard__card-name {
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
  color: #222;
}
.PayCourseCard__card-teacher {
  font-weight: normal;
  font-size: 12px;
  line-height: 18px;
}
.PayCourseCard__card-price {
  font-weight: bold;
  font-size: 24px;
  line-height: 36px;
}
.PayCourseCard__card-box {
  display: flex;
  align-items: center;
}
</style>
