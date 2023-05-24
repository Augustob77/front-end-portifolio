<template>
  <div>
    <Header />
    <About />
    <!-- <Contact /> -->
    <Projects />
    <Services />
  </div>
</template>

<script>
import About from '../components/About.vue'
// import Contact from '../components/Contact.vue'
import Projects from '../components/Projects.vue'
import Services from '../components/Services.vue'
import Header from '@/components/Header.vue'

export default {
  name: 'Index',
  components: {
    Header,
    About,
    // Contact,
    Projects,
    Services,
  },
}
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>
