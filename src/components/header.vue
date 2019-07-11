<template>
  <div>
    <img src="../assets/home/weiner.jpg" alt="Weiner Dog" title="Weiner Dog">
    <div>
      <h1>{{ greeting }} </h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'pageHeader',
  props: {
    greeting: String
  }
}
</script>

<style scoped>
  h1 {
    border: 2px solid blue;
  }
</style>
