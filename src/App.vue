<template>
  <div id="app">
    <img src="./assets/logo.png">
    <MasterPage />
  </div>
</template>

<script>
import MasterPage from './components/main/MasterPage.vue'

export default {
  name: 'app',
  components: {
    MasterPage
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
