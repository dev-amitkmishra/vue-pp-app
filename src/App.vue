<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <grid :data="gridData" :columns="gridColumns"></grid>
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld.vue';
  import Grid from './components/Grid.vue'

  export default {
    name: 'app',
    components: {
      HelloWorld,
      Grid
    },
    data() {
      return {
        gridData: [{
            name: 'Amit Mishra',
            location: 'India'
          }
        ],
        gridColumns: ['name', 'location'],
      }
    },
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>