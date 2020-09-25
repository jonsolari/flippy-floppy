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
  width: 200px;
  height: 200px;
  margin: 5px;
}

.text{
  color: white;
  font-size: 1.9rem;
  font-family: helvetica;
  font-weight: bold;
  margin: auto;
}

</style>
