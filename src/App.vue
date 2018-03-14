<template>
  <div id="app">
    <Header />
    <Content />
  </div>
</template>

<script>
import Header from './components/main/Header.vue'
import Content from './components/main/Content.vue'

export default {
  name: 'app',
  components: {
    Header,
    Content
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
