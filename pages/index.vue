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
