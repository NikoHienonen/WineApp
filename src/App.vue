<template>
  <div id="app">
    <Header />
    <Wines v-bind:wines="wines" />
  </div>
</template>

<script>

import Wines from './components/Wines';
import Header from './components/Header';

export default {
  name: 'app',
  components: {
    Header
    , Wines
  },
  data() {
    return {
      wines: [
        {id: 1111
        , name: 'Santa Helena Varietal Sauvignon Blanc'
        , color: 'white'
        , stars: 3
        , comment: 'Dry, yet very refreshing, ideal for summer days, soda-like texture.'
        , img: 'santahelena.jpg'
        }
        ,{id: 1112
        , name: 'Moss Brothers Cabernet Merlot'
        , color: 'red'
        , stars: 5
        , comment: 'Full-bodied, dark, excellent by itself, perfect with red meat.'
        , img: 'mossbros.jpg'
        }
        ,{id: 1113
        , name: 'Gato Negro Cabernet Sauvignon'
        , color: 'red'
        , stars: 1
        , comment: 'Very thin, juice-like texture. Tastes like grapejuice gone bad.'
        , img: 'gatonegro.png'
        }
      ]
    }
  }
}
</script>

<style>
:root {
  --darkred: #5D001E;
  --lightgrey: #E3E2DF;
  --lightpink: #E3AFBC;
  --darkpink: #9A1750;
  --pink: #EE4C7C;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
#app {

}
</style>
