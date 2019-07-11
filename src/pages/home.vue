<template>
  <div>
    <pageHeader greeting="Home" />
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import pageHeader from '../components/header.vue'

export default {
  name: 'home',
  components: {
    pageHeader
  },
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>
