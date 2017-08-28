<template>
  <div id="app">
    <loading :animation="animationName"></loading>
  </div>
</template>

<script>
import loading from './components/loading.vue'
export default {
  name: 'app',
  data() {
    return {
      animationName: 'square'
    }
  },
  components: {
    loading
  }
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

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
