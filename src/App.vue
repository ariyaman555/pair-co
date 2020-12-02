<template>
  <div id="app">
    <PairCo/>
  </div>
</template>

<script>
import PairCo from './components/PairCo.vue'

export default {
  name: 'App',
  components: {
    PairCo
  }
}
</script>

<style lang="scss">
@font-face {
  font-family: Supermarket;
  src: url("./assets/fonts/supermarket.ttf") format("truetype");
}
@font-face {
  font-family: Kanit;
  src: url("./assets/fonts/Kanit-Regular.ttf") format("truetype");
}
@font-face {
  font-family: Arabica;
  src: url("./assets/fonts/Arabica.ttf") format("truetype");
}
html, body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Supermarket;
}
</style>
