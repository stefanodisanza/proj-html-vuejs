<template>
  <div>
    <Header />
    <Hero />
    <Consultans />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Consultans from './components/Consultans.vue';

export default {
  components: {
    Header,
    Hero,
    Consultans
  }

}
</script>

<style lang="scss">
@use './style/general.scss';
</style> 
