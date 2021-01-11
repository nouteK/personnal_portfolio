<template>
  <div id="app">
    <router-view/>
    <Footer />
  </div>
</template>
<script>
import Footer from './components/Footer.vue'

export default {
  components : {
    Footer
  }
}

</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500&display=swap');
body {
  padding: 0;
  margin: 0;
  background-color:black;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}

/* #nav a.router-link-exact-active {
  color: #42b983;
} */

</style>
