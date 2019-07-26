<template>
  <div id="app">
    <social />
    <mainNav :navItems="[{name: 'Home', url: '../home'}, {name: 'Kitchen', url: '../kitchen'}, {name: 'Pet', url: '../pet'}, {name: 'Housewares', url: '../housewares'}]"/>
    <home msg="Hello"/>
  </div>
</template>

<script>
import mainNav from './components/nav/nav.vue'
import home from './pages/home.vue'
import social from './components/nav/social.vue'

export default {
  name: 'app',
  components: {
    home,
    mainNav,
    social
  }
}
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  margin: 3em 5em 0 5em;
  border: 2px solid black;
}
</style>
