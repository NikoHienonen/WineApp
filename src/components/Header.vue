<template>
  <header>
    <h1>Wine App</h1>
  </header>
</template>

<script>
import WineCard from './WineCard';

export default {
  name: "Header"
}
</script>
<style scoped>
  header {
    width: 100%;
    background-color: var(--darkred);
    color: white;
    padding: 0.25rem 0.5rem;
  }
</style>
