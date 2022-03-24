<template>
  <div id="app">
    <HeaderSpotify></HeaderSpotify>
    <MainSpotify></MainSpotify>
  </div>
</template>

<script>
import HeaderSpotify from './components/HeaderSpotify.vue'
import MainSpotify from './components/MainSpotify.vue'

export default {
  name: 'App',
  components: {
    HeaderSpotify,
    MainSpotify,
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "./assets/styles/style.scss"
</style>

/* https://flynn.boolean.careers/exercises/api/array/music */