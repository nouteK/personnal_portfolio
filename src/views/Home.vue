<template>
  <div class="vertical-center">
  <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-6">
          <img :src="profile_image" class="img-fluid profil_img" alt="Photo_de_profile">
        </div>
        <div class="col-lg-6 col-md-6">
          <h1 class="title">Pawel <span class="yellow">TROFIMIUK</span></h1>
          <h3 class="subtitle align-right">//Développeur Web Full-Stack</h3>
          <img :src="profile_image_mobile" class="img-fluid profil_img_mobile mx-auto" alt="Photo_de_profil_Mobile">
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Labore, maxime fugiat! Possimus sunt necessitatibus iusto nisi a, minima et. At debitis blanditiis laborum saepe provident magnam deserunt fuga obcaecati earum!</p>
          <ul class="nav flex-column mt-5">
            <li class="nav-item">
              <router-link to="/" class="nav-link">/Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/" class="nav-link">/Projets</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">/Contact</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">/CV</router-link>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  data: function(){
    return {
      profile_image: 'https://picsum.photos/id/1005/500/600',
      profile_image_mobile: 'https://picsum.photos/id/1005/200/300'
    }
  },
  components: {

  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;500&display=swap');
* {
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
}
.profil_img_mobile{
  display: none;
}
h1{
  font-family: 'Roboto', sans-serif;
  font-size: 60px;
  font-weight: 500;
  text-align: right;
}
.yellow{
  color: yellow;
  font-weight: 500;
}
.subtitle{
  font-size: 20px;
  color: grey;
  margin-bottom: 30px;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;
  text-align: right;
}
.vertical-center {
  min-height: 90vh;
  display: flex;
  align-items: center;
}
.nav-link{
  width: 2em;
}
@media screen and (max-width: 767px){
  h1{
    font-size: 2.2em;
    text-align: center;
    padding-top: 20px;
  }
  .nav-link{
    width: 100%;
  }
  .profil_img{
    display: none;
  }
  .subtitle{
    text-align: center;
    font-size: 16px;
}
  .profil_img_mobile{
    display: flex;
    margin-bottom: 2em;
  }
}
</style>
