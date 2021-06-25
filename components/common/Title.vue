<template>
  <div class="content-title">
    <h1 class="text-center title-c">
      {{ value }}
    </h1>
  </div>
</template>

<script>
export default {
  name: 'Title',
  props: {
    value: {
      type: String,
      default: 'Title',
    },
  },
}
</script>

<style lang="css" scoped>
h1 {
  margin-bottom: 0;
}
.title-c {
  font-size: 40px;
  font-weight: 900;
  color: #6dadef;
  @media (max-width: 768px) {
    font-size: 1.125rem;
  }
}
</style>
