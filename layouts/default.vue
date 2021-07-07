<template>
  <div>
    <TopBar class="d-md-block" />
    <NavBar />
    <Nuxt />
    <Footer />
  </div>
</template>
<script>
import TopBar from '@/components/core/TopBar'
import NavBar from '@/components/core/NavBar'
import Footer from '@/components/core/Footer/index'
export default {
  components: { NavBar, TopBar, Footer },
}
</script>

<style lang="css">
.section {
  padding: 60px 15px;
}
</style>
