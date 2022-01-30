<template>
<div>
<template>
  <v-card>
    <v-tabs
      color="deep-purple accent-4"
      right
    >
      <v-tab>Landscape</v-tab>
      <v-tab>City</v-tab>
      <v-tab>Abstract</v-tab>
    </v-tabs>
  </v-card>
</template>
</div>
</template>
<script lang="ts">
import Vue from 'vue'
// import qCard from '../qoute/qCard.vue'
export default Vue.extend({
    components: {
      // qCard
  },
   data: () => ({
      items: [
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me 2' },
      ],
    }),
})
</script>

<style>

</style>