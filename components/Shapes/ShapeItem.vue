<template>
  <div>
    <h1 class="shape-item-header">All Oval Items: (6)</h1>

    <div class="grid-container">
      <div class="box">
        <div class="oval"></div>
      </div>
      <div class="box">
        <div class="oval"></div>
      </div>
      <div class="box">
        <div class="oval"></div>
      </div>
      <div class="box">
        <div class="oval"></div>
      </div>
      <div class="box">
        <div class="oval"></div>
      </div>
      <div class="box">
        <div class="oval"></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.shape-item-header {
  font-size: 18px;
  font-weight: 700;
  margin-bottom: 2rem;
  color: $dark-gray;
}
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 40px;
  margin-bottom: 2rem;

  @include mobile {
    grid-template-columns: repeat(1, 1fr);
  }
   @include tablet {
    grid-template-columns: repeat(1, 1fr);
    place-items: center;
  }
}
.box {
  /* width: 100%; */
   @include tablet {
      width: 80%;
  }
  height: 100px;
  background-color: $white;
  cursor: pointer;
  padding: 30px;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease-in-out;
}
.oval {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 1px solid #e1e5e9;
  background-color: $red;
  cursor: pointer;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease-in-out;
}
.active {
  background-color: #d7d7f1;
}
</style>
<script>
export default {
  name: 'ShapeItem'
}
</script>