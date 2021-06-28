<template>
  <div class="Skills">
    <b-container>
      <div class="d-flex pt-5">
        <img
          style="max-width: 100%; padding-top: 90px"
          :src="require('@/assets/img/skills/skills.png')"
          alt=""
        />
      </div>
    </b-container>
  </div>
</template>

<script>
// import SkillsCard from '@/components/partials/cards/SkillsCard.vue'
export default {
  name: 'Skills',
  // components: { SkillsCard },
}
</script>

<style lang="css" scoped>
.Skills {
  background-color: #558ae8;
  min-height: 637px;
}
</style>
