<template>
  <div id="app">
    <mainNav :navItems="[{name: 'Home', url: '../home'}, {name: 'Kitchen', url: '../kitchen'}, {name: 'Pet', url: '../pet'}, {name: 'Housewares', url: '../housewares'}]"/>
    <home msg="Hello"/>
  </div>
</template>

<script>
import mainNav from './components/nav.vue'
import home from './pages/home.vue'

export default {
  name: 'app',
  components: {
    home,
    mainNav
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  margin: 3em 5em 0 5em;
  border: 2px solid black;
}
</style>
