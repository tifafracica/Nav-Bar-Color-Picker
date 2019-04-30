<template>
  <div id="app">
    <NavBar />
    
    
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import ColorSwatches from './components/ColorSwatches.vue'
import "vue-swatches/dist/vue-swatches.min.css"


export default {
  name: 'app',
  components: {
    NavBar,
    
  }
  
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  
}
</style>
