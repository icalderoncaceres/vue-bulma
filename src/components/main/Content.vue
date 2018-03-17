<template>
    <div class="container">
      <div class="columns">
        <div class="column is-3">
          <VerticalMenu />
        </div>
        <div class="column is-9">
          <Breadcumb />
          <Greeting user="Iván" message="Welcome to my page" />
          <ResumenSection />
          <div class="columns">
            <div class="column is-6">
                <Events />
            </div>
            <div class="column is-6">
              <div class="card">
                  <Searcher title="Buscador 1" />
              </div>
              <div class="card">
                  <Searcher  title="Buscador 2"/>
              </div>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
import Searcher from '../form/Searcher.vue'
import VerticalMenu from '../panel/VerticalMenu.vue'
import Events from '../form/Events.vue'
import Breadcumb from '../panel/Breadcumb.vue'
import Greeting from '../form/Greeting.vue'
import ResumenSection from '../form/ResumenSection.vue'
export default {
  name: 'Content',
  props: {
  },
  components:{
    Searcher,
    VerticalMenu,
    Events,
    Breadcumb,
    Greeting,
    ResumenSection
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
