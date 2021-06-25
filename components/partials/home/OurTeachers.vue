<template>
  <div class="OurTeachers">
    <b-container>
      <div>
        <h1 class="text-center">
          {{ title }}
        </h1>
      </div>
      <div>
        <TeachersCard />
      </div>
    </b-container>
  </div>
</template>

<script>
import TeachersCard from '@/components/partials/cards/TeachersCard.vue'
export default {
  name: 'OurTeachers',
  components: { TeachersCard },
  data() {
    return {
      title: 'Nuestros Profesores',
    }
  },
}
</script>

<style lang="css" scoped>
.OurTeachers {
  background-color: #fff;
}
</style>
