<template>
  <div id="app">
    <firstfile msg="hello I am shridhi " />
    <cube></cube>
  </div>
</template>

<script>
import firstfile from './components/firstfile.vue'
import cube from './components/cube.vue'


export default {
  name: 'App',
  components: {
    firstfile,
    cube
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
