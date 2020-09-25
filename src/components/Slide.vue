<template>
<div class="box">
  <p class="text">{{this.title}}</p>
</div>
</template>

<script>
export default {
  name: 'Slide',
  props: {
    title: {
      type: String
    }
  }
}
</script>


<style scoped>
.box{
  display: flex;
  background-color: red;
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
