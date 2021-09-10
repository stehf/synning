<template>
  <div id="app">
    <Weekdays />
  </div>
</template>
<script>
  import Weekdays from './components/Weekdays.vue'
   export default {
    name: 'app',
    components: {
      Weekdays
    }
  }
</script>
<style>
  body {
    margin:  0;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
  }
</style>