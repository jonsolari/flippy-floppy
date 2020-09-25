<template>
  <div id="app">
    <Slide title="VIDEOGAME" /> <Slide title="SANDWICH"/> <Slide title="DIAMONDS" />
  </div>
</template>

<script>
import Slide from './components/Slide.vue'

export default {
  name: 'App',
  components: {
    Slide
  }
}
</script>

<style>
#app {
  display: flex;
  flex-direction: row;
}
</style>
