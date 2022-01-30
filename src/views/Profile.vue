<template>
  <div class="container">
      <h1>Profile</h1>
      <div class="card"><q-card /></div>

  </div>
</template>

<script>
// @ is an alias to /src
import qCard from '../components/qoute/qCard.vue'
export default {
  name: 'Profile',
  components: {
      qCard
  }
}
</script>


<style>
.container {
  width: 20%;
  margin: 0 auto;
}

</style>
