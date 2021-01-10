<template>
  <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <router-link to="/" class="navbar-brand white">Home</router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/" class="nav-link ez">Projets</router-link>
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

<style>

</style>