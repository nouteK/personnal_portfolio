<template>
  <vueper-slides fade autoplay :pauseOnHover="false" :arrows="false" :bullets="false">
      <vueper-slide v-for="(slide, i) in slides" :key="i" :content="slide.content"/>
  </vueper-slides>
</template>

<script>
import {VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'
export default {
    data:() => ({
        slides: [
            {
                content: '<img src="https://storage.googleapis.com/img_kat/js4.png" class="img_fluid"/>'
            },
            {
                content: '<img src="https://storage.googleapis.com/img_kat/test.png" class="img_fluid"/>'
            },
            {
                content: '<img src="https://storage.googleapis.com/img_kat/symfony3.png" class="img_fluid"/>'
            },
            {
                content: '<img src="https://storage.googleapis.com/img_kat/vuejs2.png" class="img_fluid"/>'
            },
            {
                content: '<img src="https://storage.googleapis.com/img_kat/ps2.png" class="img_fluid"/>'
            },
            {
                content: '<img src="https://storage.googleapis.com/img_kat/sql.png" class="img_fluid"/>'
            }
        ],
    }),
    components: {
        VueperSlides, VueperSlide
    },
}
</script>

<style>
/* .carousel {
    max-width: 200px;
    max-height: 200px;
} */
/* .vueperslide__content img{
    /* height: 100px;
    width: auto; */

</style>