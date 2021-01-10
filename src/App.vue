<template>
  <div id="app">
    
    <router-view/>
    <footer class="text-center text-lg-start">
      <div class="text-center m-4">
        Copyright welpaCorporation
      </div>
    </footer>
  </div>
</template>

<style>
body {
  padding: 0;
  margin: 0;
  background-color:black;
}
.white{
  color: white !important;
}
.nav-link{
  color: yellow !important;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

</style>
