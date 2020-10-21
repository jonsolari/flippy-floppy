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

.leftred{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 70% 80%, red, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}

.leftblue{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 70% 80%, steelblue, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}

.middlered{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 50% 70%, red, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}

.middleblue{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 50% 70%, steelblue, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}

.rightred{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 30% 80%, red, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}

.rightblue{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-image: radial-gradient(circle at 30% 80%, steelblue, black);
  width: 33vw;
  height: 30vw;
  position: relative;
  margin: .8vw;
}


.text{
  color: lightgrey;
  letter-spacing: -5px;
  display: flex;
  align-self: center;
  position: absolute;
  font-size: 4.8vw;
  font-family: helvetica;
  font-weight: bold;
  text-align: center;
  bottom: 30%;
}

</style>
