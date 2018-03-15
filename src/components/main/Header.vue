<template>
      <!-- START NAV -->
      <nav class="navbar is-white">
        <div class="container">
          <div class="navbar-brand">
            <a class="navbar-item brand-text" target="_blank" href="https://icalderoncaceres.github.io">
              Ivan Calderon
            </a>
            <div class="navbar-burger burger" data-target="navMenu">
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>
          <div id="navMenu" class="navbar-menu">
            <div class="navbar-start">
              <a class="navbar-item" :href="option.target" v-for="option in options">
                {{option.title}}
              </a>
            </div>

          </div>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'Header',
  props: {
  },
  data:function(){
    return {
      options:[
        {id:0,title:'Home',target:'#'},
        {id:1,title:'Documentation',target:'#'},
        {id:2,title:'Settings',target:'#'}
      ]    
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
