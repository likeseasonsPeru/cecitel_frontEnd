<template>
  <div>
    <img :src="image" alt="Banner" />
  </div>
</template>

<script>
export default {
  name: 'BannerTop',
  props: {
    image: {
      type: String,
      default: 'Hola',
    },
  },
}
</script>

<style scoped>
img {
  width: 100%;
  max-height: 412px;
}
</style>
