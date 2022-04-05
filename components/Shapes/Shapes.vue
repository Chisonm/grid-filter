<template>
  <div class="shapes">
      <h1 class="shapes-header">Shapes</h1>

      <div class="flex-container">
        <button class="shape active">Oval</button>
        <button class="shape">Round</button>
        <button class="shape">Triangle</button>
        <button class="shape">Square</button>
        <button class="shape">Rectangle</button>
      </div>
  </div>
</template>

<style lang="scss" scoped>
.shapes-header{
  font-size: 18px;
  font-weight: 700;
  margin-bottom: 2rem;
  color: #329ef7;
}
.flex-container{
  display: flex;
  align-items: center;
  margin-bottom: 2rem;
  scroll-behavior: smooth;
  overflow-x: auto;
  
}
.flex-container::-webkit-scrollbar {
  width: 0px;
  height: 0px;
}
.shape{
  width: 100px;
  height: 30px;
  border-radius: 20px;
  border: 1px solid #e1e5e9;
  background-color: #F0F0F0;
  color: #000;
  font-size: 15px;
  font-weight: 700;
  margin-right: 2rem;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
  &:hover{
    background-color: #d7d7f1;
    color: #000;
  }
}
.active{
    background-color: #d7d7f1;
}
</style>
<script>
export default {
  name: 'Shapes'
}
</script>