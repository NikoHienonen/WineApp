<template>
  <div class="card">
    <img v-bind:alt="wine.name" v-bind:src="image"/>
    <div class="card-info">
      <h3>{{wine.name}}</h3>
      <p>Color: {{wine.color}}</p>
      <p>Stars: {{wine.stars}}</p>
      <p>{{wine.comment}}</p>
  </div>
  </div>
</template>

<script>
export default {
  name: 'WineCard'
  , props: ["wine"]
  , data () {
  return {
    image: require('@/assets/'+this.wine.img)
  }
}
}
</script>

<style scoped>
.card {
  /* Add shadows to create the "card" effect */
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  margin: 1rem;
  padding: 1rem;
}

/* On mouse-over, add a deeper shadow */
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

/* Add some padding inside the card container */
.card-info {
  padding: 1rem 0;
}
img {
  max-width: 100%;
  margin: 0 auto;
}
</style>

