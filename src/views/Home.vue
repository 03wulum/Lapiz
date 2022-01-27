<template>
  <div>
    <hello-world/>
      <nav-bar/>
      <h1>
         Home view
      </h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import NavBar from '../components/Nav/NavBar.vue'
import HelloWorld from '../components/HelloWorld.vue'
// import navigation from '../components/Nav/NavBar.vue'
export default Vue.extend({
    components: {
    NavBar,
    HelloWorld,
  },
})
</script>

