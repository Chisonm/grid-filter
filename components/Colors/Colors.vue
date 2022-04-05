<template>
  <div class="color">
      <h1 class="shapes-header">Colors</h1>

      <div class="flex-container">
        <button class="colors red"></button>
        <button class="colors blue"></button>
        <button class="colors green"></button>
        <button class="colors yellow"></button>
        <button class="colors lightblue"></button>
        <button class="colors gray"></button>
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
}
.colors{
  width: 50px;
  height: 50px;
  @include mobile{
    height: 25px;
  }
  border-radius: 50%;
  border: 1px solid $dark-gray;
  margin-right: 2rem;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
}
.red{
    background-color: $red;
    &:hover{
      background-color: darken($color: $red, $amount: 5%);
    }
}
.blue{
    background-color: $blue;
     &:hover{
      background-color: lighten($color: $blue, $amount: 5%);
    }
}
.green{
    background-color: $green;
     &:hover{
      background-color: lighten($color: $green, $amount: 5%);
    }
}
.yellow{
    background-color: $yellow;
      &:hover{
      background-color: lighten($color: $yellow, $amount: 5%);
    }
}
.lightblue{
    background-color: $light-blue;
      &:hover{
      background-color: lighten($color: $light-blue, $amount: 5%);
    }
}
.gray{
    background-color: $gray;
      &:hover{
      background-color: lighten($color: $gray, $amount: 5%);
    }
}
</style>
<script>
export default {
  name: 'Colors'
}
</script>
