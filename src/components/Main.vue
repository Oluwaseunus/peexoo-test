<template>
  <div class="main">
    <Navbar />
    <div class="availability">Availability Ting</div>
  </div>
</template>

<script>
import Navbar from './Navbar';

export default {
  components: {
    Navbar
  }
};
</script>

<style lang="scss" scoped>
.main {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 0.8fr 5fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  background: #fffdf9;
}

.nav {
  box-shadow: 0 1px 4px 0 rgba(204, 204, 204, 0.5);
}
</style>
