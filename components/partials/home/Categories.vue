<template>
  <div class="Categories">
    <b-container>
      <div>
        <div class="mb-5">
          <Title :value="title" />
        </div>
        <div class="d-flex">
          <div v-for="(card, index) in cards" :key="index">
            <CategoryCard :card="card" />
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import Title from '@/components/common/Title.vue'
import CategoryCard from '@/components/partials/cards/CategoryCard.vue'

export default {
  name: 'Categories',
  components: { CategoryCard, Title },
  data() {
    return {
      title: 'Categorías',
      cards: [
        {
          title: 'Semipresenciales',
          text: 'Some quick example text to build on the card title and make up the bulk of the cards content.',
          image: require('@/assets/img/semipresenciales_home.png'),
        },
        {
          title: 'Enlatados',
          text: 'Some quick example text to build on the card title and make up the bulk of the cards content.',
          image: require('@/assets/img/enlatados_home.png'),
        },
        {
          title: 'Corporativo',
          text: 'Some quick example text to build on the card title and make up the bulk of the cards content.',
          image: require('@/assets/img/corporativo_home.png'),
        },
      ],
    }
  },
}
</script>

<style>
.Categories {
  background-image: url('@/assets/img/categories/category-right.svg'),
    url('@/assets/img/categories/category-left.svg');
  background-repeat: no-repeat, no-repeat;
  background-position: left, right;
  height: 100%;
  width: 100%;
}
.Categories-title {
  font-weight: bold;
  color: #5d8eca;
}
</style>
