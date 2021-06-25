<template>
  <div class="footer-component pt-3">
    <footer>
      <div class="body-footer">
        <div class="text-md-left container-footer">
          <section-desktop />
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import SectionDesktop from '@/components/core/Footer/SectionDesktop'

export default {
  name: 'Footer',
  components: { SectionDesktop },
}
</script>
<style lang="css" scoped>
.footer-component {
  background-color: #222;
  color: #fff;
  height: 250px;
}
</style>
