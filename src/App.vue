<template>
  <div id="app">
    <Slide class="left" title="VIDEOGAME" /> <Slide class="middle" title="SANDWICH"/> <Slide class="right" title="DIAMONDS" />
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
