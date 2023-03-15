<template>
  <div>
    <Header />
    <Hero />
    <Consultans />
    <About />
    <Project />
    <Testimonial />
    <Blog />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Consultans from './components/Consultans.vue';
import About from './components/About.vue'
import Project from './components/Project.vue';
import Testimonial from './components/Testimonial.vue';
import Blog from './components/Blog.vue';

export default {
  components: {
    Header,
    Hero,
    Consultans,
    About,
    Project,
    Testimonial,
    Blog
  }

}
</script>

<style lang="scss">
@use './style/general.scss';
</style> 
