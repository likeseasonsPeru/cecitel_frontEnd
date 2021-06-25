<template>
  <div class="CategoryCard">
    <b-card
      :title="card.title"
      :img-src="card.image"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem"
      class="mx-3 CategoryCard_card"
    >
      <b-card-text>
        {{ card.text }}
      </b-card-text>

      <b-button href="#" pill class="px-4">Ver más</b-button>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'CategoryCard',
  props: {
    card: {
      type: Object,
      default() {
        return {
          text: 'lorem ipsum 20',
          title: 'Semipresenciales',
          image: 'https://picsum.photos/600/300/?image=25',
        }
      },
    },
  },
}
</script>
<style lang="css" scoped>
.CategoryCard {
  background-color: #fff;
}
.CategoryCard_card {
  border-radius: 30px;
  box-shadow: 0 2px #7bbbef;
}
</style>
