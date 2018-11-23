<template>
  <div id="app">
    <Header id="header" />
    <HomePage />
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue';
import Header from './components/Header.vue';

export default {
  name: 'app',
  components: {
    Header,
    HomePage,
  },
};
</script>

<style>
#app {
  height: 100vh;
  font-family: 'ABeeZee', 'Helvetica', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background: rgb(89, 177, 250);
  margin: 0 15%;
  padding: 0 2%;
}

#header {
  margin-bottom: 50px;
}
</style>
