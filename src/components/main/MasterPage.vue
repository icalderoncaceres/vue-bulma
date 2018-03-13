<template>
  <Header />
</template>

<script>
import MasterPage from './components/main/MasterPage.vue'
export default {
  name: 'MasterPage',
  props: {
    msg: String
  },
  components:{
    Header
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
