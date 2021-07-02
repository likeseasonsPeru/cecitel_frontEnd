<template>
  <b-card
    :img-src="item.image"
    img-alt="Image"
    img-top
    tag="article"
    class="CourseCard mx-3 mb-4"
  >
    <div class="CourseCard__head">
      <h6 class="CourseCard__title">{{ item.title }}</h6>
      <img :src="require('~/components/svg/icons/heart.svg')" alt="shop icon" />
    </div>
    <b-card-text class="CourseCard__paragraph">
      {{ item.paragraph }}
    </b-card-text>
    <div class="d-flex">
      <img :src="require('@/assets/img/courses/teacher.svg')" alt="Teacher" />
      <div class="ml-1">
        <b> Nombre y Apellidos</b> <br />
        Cargo
      </div>
    </div>
    <b-button pill class="CourseCard__button"
      ><img :src="require('~/components/svg/icons/shop.svg')" alt="shop icon"
    /></b-button>
  </b-card>
</template>

<script>
export default {
  name: 'CourseCard',
  props: {
    item: {
      type: Object,
      default() {
        return {
          image: 'https://picsum.photos/600/300/?image=25',
          title: 'Card Title',
          paragraph:
            "Some quick example text to build on the card title and make up the bulk of the card's content.",
        }
      },
    },
  },
}
</script>

<style lang="css" scoped>
.card {
  max-width: 250px;
  max-height: 400px;
  border: none;
}
.CourseCard {
  background: #fafafa;
  border-radius: 20px;
}
.CourseCard:hover {
  box-shadow: 0 6px 15px -7px #929292;
}
.CourseCard__head {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #e2e2e2;
}
.CourseCard__title {
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
}
.CourseCard__button {
  width: 101px;
  height: 35px;
  border: none;
  background: linear-gradient(270deg, #7bbbef 2.04%, #4275d2 97.45%);
  float: right;
}
.CourseCard__paragraph {
  font-size: 13px;
  line-height: 18px;
}
</style>
