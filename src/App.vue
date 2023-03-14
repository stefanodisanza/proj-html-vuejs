<template>
  <div>
    <Header />
    <Hero />
    <Consultans />
    <About />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Consultans from './components/Consultans.vue';
import About from './components/About.vue'

export default {
  components: {
    Header,
    Hero,
    Consultans,
    About
  }

}
</script>

<style lang="scss">
@use './style/general.scss';
</style> 
