<template>
<div>
  <Home/>
  <NavBar/>
</div>
 
</template>

<script lang="ts">
import Vue from 'vue';
import NavBar from './components/Nav/NavBar.vue';
import Home from './views/Home.vue';

export default Vue.extend({
  name: 'App',

  components: {
    Home,
    NavBar,
  },

  data: () => ({
    //
  }),
});
</script>
