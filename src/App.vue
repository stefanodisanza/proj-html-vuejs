<template>
  <div>
    <Header />
    <Hero />
    <Consultans />
    <About />
    <Project />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Consultans from './components/Consultans.vue';
import About from './components/About.vue'
import Project from './components/Project.vue';

export default {
  components: {
    Header,
    Hero,
    Consultans,
    About,
    Project
  }

}
</script>

<style lang="scss">
@use './style/general.scss';
</style> 
