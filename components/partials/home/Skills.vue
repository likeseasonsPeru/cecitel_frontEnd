<template>
  <div class="Skills">
    <b-container>
      <div class="d-flex">
        <div v-for="item in 4" :key="item">
          <SkillsCard />
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import SkillsCard from '@/components/partials/cards/SkillsCard.vue'
export default {
  name: 'Skills',
  components: { SkillsCard },
}
</script>

<style lang="css" scoped>
.Skills {
  background-color: #558ae8;
}
</style>
