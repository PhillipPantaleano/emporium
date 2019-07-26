<!--
  Need to figure out a better way to do nav
-->

<template>
  <div class="main-nav">
    <div class="nav-welcome">
      <span>Welcome to the Wiener Emporium</span>
    </div>
    <div class="nav">
      <a :href="item.url" title="" v-for="item in navItems" :key="item" class="nav-a">
        <span>
          {{ item.name }}
        </span>
      </a>
    </div>
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
  display: flex;
  flex-flow: row wrap;
  width: 100%;
  color: white;
  background-color: #003366;
  padding: 20px 0;
}

.nav-welcome {
  width: 40%;
  font-size: 24px;
}

.nav {
  display: flex;
  flex-direction: row;
  width: 60%;
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
