<template>
<div :class="this.class">
  <p class="text">{{this.title}}</p>
</div>
</template>

<script>
export default {
  name: 'Slide',
  props: {
    title: {
      type: String
    }, 
    class: {
      type: String
    }
  }
}
</script>


<style scoped>

.left{
  display: flex;
  background-image: radial-gradient(circle at bottom right, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  /* position: relative; */
  margin: 8px;
}

.middle{
   display: flex;
  background-image: radial-gradient(circle at bottom center, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  /* position: relative; */
  margin: 8px;
}

.right{
   display: flex;
  background-image: radial-gradient(circle at bottom left, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  /* position: relative; */
  margin: 8px;
}

.text{
  color: white;
  position: absolute;
  font-size: 4rem;
  font-family: helvetica;
  font-weight: bold;
  text-align: center;
  top: 20%;
  
  
  
}

</style>
