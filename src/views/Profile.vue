<template>
  <div class="container">
      <div class="card-profile">
        <q-card  @toggleReply="toggleReply" :isQreplyToggled=isQreplyToggled>
        </q-card >
      </div>

  </div>
</template>

<script>
// @ is an alias to /src
import qCard from '../components/qoute/qCard.vue'
export default {
  name: 'Profile',
  components: {
      qCard
  },
      data: () => ({
        isQreplyToggled: false,
    }),
  methods: {
    toggleReply() {
      this.isQreplyToggled = !this.isQreplyToggled
    }
  }
}
</script>
<style>
.container {
  display: grid;  
    grid-template-columns: 1fr 1fr 1fr;  
    grid-template-rows: 50px 50px;  
}

.card-profile {
  grid-column-start: 2;
  margin: auto;
}
</style>
