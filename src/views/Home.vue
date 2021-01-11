<template>
  <div class="vertical-center">
  <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-6">
          <img :src="profile_image" class="img-fluid profil_img" alt="Photo_de_profile">
        </div>
        <div class="col-lg-6 col-md-6">
          <h1 class="title">Pawel <span class="yellow">TROFIMIUK</span></h1>
          <h3 class="subtitle my-n5 align-right">//Développeur Web Full-Stack</h3>
          <img :src="profile_image_mobile" class="img-fluid profil_img_mobile mx-auto" alt="Photo_de_profil_Mobile">
          <p class="desc">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Labore, maxime fugiat! Possimus sunt necessitatibus iusto nisi a, minima et. At debitis blanditiis laborum saepe provident magnam deserunt fuga obcaecati earum!</p>
          <ul class="nav flex-column mt-4">
            <li class="nav-item">
              <router-link to="/" class="nav-link">./Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/projets" class="nav-link">./Projets</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">./Contact</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">./CV</router-link>
            </li>
          </ul>
          <Slides/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Slides from "../components/Slides.vue"
  // @ is an alias to /src


export default {

  name: 'Home',
  data(){
    return {
      profile_image: 'https://picsum.photos/id/1005/500/600',
      profile_image_mobile: 'https://picsum.photos/id/1005/200/300'
    };
  },
  components: {
    Slides
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500&display=swap');
* {
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
}
.nav-link{
  color: yellow !important;
}
.nav-link:hover{
  color: white !important;
}
hr{
  height: 2px;
}
.profil_img_mobile{
  display: none;
}
h1{
  font-family: 'Roboto', sans-serif;
  font-size: 2.8em;
  font-weight: 300;
  text-align: left;
}
.yellow{
  color: yellow !important;
  font-weight: 500;
}
.subtitle{
  font-size: 1.1em;
  color: grey;
  margin-bottom: 30px;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
  text-align: left;
}
.vertical-center {
  min-height: 90vh;
  display: flex;
  align-items: center;
}
.desc{
  text-align: left;
}
.nav-link{
  width: 1em;
  padding-left: 0;
}
@media screen and (max-width: 767px){
  h1{
    font-size: 2.2em;
    text-align: left;
    padding-top: 20px;
  }
  .nav-link{
    width: 100%;
  }
  .profil_img{
    display: none;
  }
  .subtitle{
    text-align: left;
    font-size: 16px;
}
  .profil_img_mobile{
    display: flex;
    margin-bottom: 2em;
  }
  ul{
    margin-bottom: 1.5em;
  }
}
</style>
