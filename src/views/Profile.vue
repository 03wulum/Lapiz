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
  /* width: 20%; */
  /* margin: 0 auto;
  display: block;
    position: absolute;
    width: 100%;
    height: auto; */
  display: grid;  
    grid-template-columns: 1fr 1fr 1fr;  
    grid-template-rows: 50px 50px;  
}

.card-profile {
  grid-column-start: 2;
  margin: auto;
    /* grid-column-end: 3; */
}
</style>
