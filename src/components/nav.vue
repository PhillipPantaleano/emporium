<template>
  <div class="main-nav">
    <a :href="item.url" title="" v-for="item in navItems" :key="item" class="nav-a">
      <span>
        {{ item.name }}
      </span>
    </a>
  </div>
</template>

<script>
export default {
  name: 'mainNav',
  props: {
    navItems: Array
  }
}
</script>

<style scoped>
.main-nav {
  width: 100%;
  background-color: #cc3399;
  padding: 20px 0;
}

a {
  list-style: none;
  margin: 5px 10px;
  padding: 10px;
  background-color: #cc3399;
  border: 1px solid black;
  text-decoration: none;
  font-size: 1.3em;
}

</style>
