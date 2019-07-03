<template>
  <div>
    <h2>Wines</h2>
    <div v-bind:key="wine.id" v-for="wine in wines">
      <WineCard v-bind:wine="wine"/>
    </div>
  </div>
</template>

<script>
import WineCard from './WineCard';

export default {
  name: "Wines"
  , components: {
    WineCard
  }
  , props: ["wines"]
}
</script>
<style scoped>

</style>
