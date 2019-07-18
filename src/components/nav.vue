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
  width: 100%;
  color: white;
  background-color: #003366;
  padding: 20px 0;
}

/* clear the floats after the div columns
- allows everything to go back to being normal */
.main-nav:after {
  content: "";
  display: table;
  clear: both;
}

.nav-welcome {
  width: 50%;
  float: left;
  font-size: 24px;
}

.nav {
  width: 50%;
  float: left;
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
