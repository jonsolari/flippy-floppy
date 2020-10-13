<template>
  <div id="app">

    <div class="slides">
      <Slide class="left" :title="this.left" /> 
      <Slide class="middle" :title="this.center"/> 
      <Slide class="right" :title="this.right" />
    </div>

    <div class="silhouette">
      <img src="./assets/VSD4.png">
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



export default {
  name: 'App',
  components: {
    Slide
  }, 
  data(){
    return{
      left: 'VIDEOGAME',
      center: 'SANDWICH',
      right: 'DIAMONDS'
    }
  }
}
</script>

<style>
body{
  background-color: black;
}
.silhouette{
  position: absolute;
  top: 9.8vh;
  left: -.5vw;
}
img{
  width: 100vw;
  /* height: auto; */
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
  text-align: center;
}
.btn{
  display: flex;
  margin: auto;
  height: 5vh;
  align-items: center;
}
</style>
