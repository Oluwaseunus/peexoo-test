<template>
  <div>
    <div class="logo"></div>
    <div class="links"></div>
    <div class="info"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
div {
  background: #4d4d4d;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.logo {
  align-items: center;
  background: url('http://peexoo.ai/images/logo.png');
  background-size: cover;
  background-position: center;
  width: 80%;
  height: 14rem;
  display: flex;
  align-self: center;
}
</style>
