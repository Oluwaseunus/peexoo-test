<template>
  <div id="app">
    <Sidebar />
    <Main />
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue';
import Main from './components/Main.vue';

export default {
  name: 'app',
  components: {
    Sidebar,
    Main
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,500&display=swap');

*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  box-sizing: border-box;
  font-size: 10px;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: grid;
  grid-template-columns: 1fr 4fr;
  grid-template-rows: 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}
</style>
