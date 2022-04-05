<template>
  <div class="header">
    <div class="header-container">
      <div class="nav">
        <div>
          <a class="logo" href>Shapes</a>
        </div>
        <div>
          <a class="auth-btn" href>Login</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.header {
  height: 50px;
  background-color: #fff;
  width: 100%;
  /* border-bottom: 1px solid #e5e5e5; */
}
.nav {
  height: 50px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header-container{
 width: 80%;
 margin: 0 auto;
  @include mobile {
  width: 90%;
  margin: 0 auto;
  }
}
</style>
<script>
export default {
  name: 'Header'
}
</script>