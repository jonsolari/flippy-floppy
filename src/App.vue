<template>
  <div id="app">

    <div class="slides">
      <Slide :class="this.leftbox" :title="this.leftText" /> 
      <Slide :class="this.middlebox" :title="this.centerText"/> 
      <Slide :class="this.rightbox" :title="this.rightText" />
    </div>

    <div class="silhouette">
      <img src="./assets/VSD5.png">
    </div>

    <div class="inputs">
      <input type="text" class="boxes" v-model="left">
      <input type="text" class="boxes" v-model="center">
      <input type="text" class="boxes" v-model="right">
    </div>

    <div class="redblue">
      <input type="radio" name="color" id="red" v-model="selected" value="red" checked>
      <label for="red" class="slidecolor">Red</label>
      <input type="radio" name="color" id="blue" v-model="selected" value="blue">
      <label for="blue" class="slidecolor">Blue</label>
    </div>

  </div>
</template>

<script>
import Slide from './components/Slide.vue'



export default {
  name: 'App',
  components: {
    Slide
  }, 
  computed: {
    leftText(){
      return this.left.toUpperCase();
    },
    centerText(){
      return this.center.toUpperCase();
    },
    rightText(){
      return this.right.toUpperCase();
    },
    leftbox(){
      return ('left' + this.selected);
    },
    middlebox(){
      return ('middle' + this.selected);
    },
    rightbox(){
      return ('right' + this.selected);
    }
  },
  data(){
    return{
      left: 'VIDEOGAME',
      center: 'SANDWICH',
      right: 'DIAMONDS',
      selected: 'red'
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
  top: 5.8vw;
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
.slidecolor{
  color: white;
}
.redblue{
  display: flex;
  margin: auto;
}
</style>
