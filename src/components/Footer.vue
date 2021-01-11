<template>
  <footer class="text-center text-lg-start">
      <div class="text-center">
        <a href="https://instagram.com/welpa_" target="_blank"><img :src="insta" alt="Instagram" class="small"></a>
        <a href="https://instagram.com/welpa" target="_blank"><img :src="linkedin" alt="Instagram" class="small"></a>
      </div>
    </footer>
</template>

<script>
export default {

    name: 'Footer',
    data(){
        return {
            insta: 'https://storage.googleapis.com/img_kat/insta_jaune.png',
            linkedin: 'https://storage.googleapis.com/img_kat/linkedin.png'
        }
    }
}
</script>

<style>
.small {
    width: 30px;
    height: auto;
    margin: 2em;
}
.small img {
    width: 50px;
    
    color: yellow;
}
</style>