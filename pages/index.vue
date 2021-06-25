<template>
  <div>
    <div>
      <Homer />
      <About />
      <Categories />
      <Skills />
      <OurTeachers />
      <Brands />
    </div>
  </div>
</template>

<script>
import Homer from '@/components/partials/home/Homer.vue'
import About from '@/components/partials/home/About.vue'
import Categories from '@/components/partials/home/Categories.vue'
import Skills from '@/components/partials/home/Skills.vue'
import OurTeachers from '@/components/partials/home/OurTeachers.vue'
import Brands from '@/components/partials/home/Brands.vue'

export default {
  name: 'Index',
  components: { Homer, About, Categories, Skills, OurTeachers, Brands },
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
