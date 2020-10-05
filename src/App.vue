<template>
  <div id="app">

    <div class="slides">
    <Slide class="left" title="VIDEOGAME" /> <Slide class="middle" title="SANDWICH"/> <Slide class="right" title="DIAMONDS" />
    </div>

    <div class="inputs">
      <input type="text" class="boxes" placeholder="LEFT">
      <input type="text" class="boxes" placeholder="CENTER">
      <input type="text" class="boxes" placeholder="RIGHT">
    </div>
    <button type="submit" class="btn">CREATE</button>

  </div>
</template>

<script>
import Slide from './components/Slide.vue'

// function data(e){
//   return e
// }

export default {
  name: 'App',
  components: {
    Slide
  }
}

// function changeHandler(e){

// }

</script>

<style>
body{
  background-color: black;
}
.slides{
  display: flex;
  flex-direction: row;
}
.inputs{
  display: flex;
  margin: auto;
}
.boxes{
  margin: 10vh auto;
  width: 20%;
  background-color: darkgrey;
}
.btn{
  display: flex;
  margin: auto;
  height: 5vh;
  align-items: center;
}
</style>
