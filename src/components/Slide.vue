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
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 70% 80%, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  position: relative;
  margin: 8px;
}

.middle{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 50% 80%, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  position: relative;
  margin: 8px;
}

.right{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 30% 80%, #f35, #F00);
  width: 33%;
  padding-top: 33%;
  position: relative;
  margin: 8px;
}

.text{
  color: white;
  display: flex;
  align-self: center;
  position: absolute;
  font-size: 8vh;
  font-family: helvetica;
  font-weight: bold;
  text-align: center;
  bottom: 30%;
}

</style>
