<template>
  <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <router-link to="/" class="navbar-brand white">Pawel <span class="yellow">TROFIMIUK</span></router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end" id="navbarSupportedContent">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/projets" class="nav-link">Projets</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">Contact</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">CV</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>

<style scoped>
.nav-link{
  color: white !important;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
}
.nav-link:hover{
  color: yellow !important;
}
.yellow {
  color: yellow;
  font-family: 'Roboto', sans-serif;
  font-weight: 500;
}
.white {
  color: white !important;
}
</style>