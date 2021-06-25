<template>
  <div>
    <b-container>
      <div class="d-flex">
        <div v-for="(brand, index) in brands" :key="index">
          <img :src="brand.image" alt="image-brand" class="mx-5" />
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'Brands',
  data() {
    return {
      brands: [
        { image: require('@/assets/img/brands/cercil.png') },
        { image: require('@/assets/img/brands/boticas_salud.png') },
        { image: require('@/assets/img/brands/clinica_miraflores.png') },
        { image: require('@/assets/img/brands/nissan.png') },
      ],
    }
  },
}
</script>
