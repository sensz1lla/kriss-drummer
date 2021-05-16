<template>
  <div id="coversVideo" class="slider-video">
    <h3 class="slider-title">Cover videos.</h3>
    <div class="line"></div>
    <VueSlickCarousel v-bind="settings">
      <div class="item">
        <iframe src="https://www.youtube.com/embed/vgKNL6gJBJ0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="item">
        <iframe src="https://www.youtube.com/embed/hfxhWGtDuYA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="item">
        <iframe src="https://www.youtube.com/embed/bbpLalxKaFg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="item">
        <iframe src="https://www.youtube.com/embed/GfPGfhRV7yA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="item">
        <iframe src="https://www.youtube.com/embed/rQd0TLePMtw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
    </VueSlickCarousel>
  </div>
</template>
 
<script>
  
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
  //import 'font-awesome/css/font-awesome.min.css'
 
  export default {
    name: 'SlideVideo',
    components: { VueSlickCarousel },
    data() {
      return {
        settings: {
          arrows: true,
          dots: true,
          autoplay: true,
          autoplaySpeed: 3000,
          //prevArrow: '<button class="prev"></button>'
        },
      }
    },
  }

</script> 

<style lang="scss">

    .slider-video {
      height: 100vh;
      min-height: 700px;
      padding: 100px 0;

      .slider-title {
        text-align: center;
      }

      .line {
        margin: 0 auto 60px;
      }

      .item {
        display: flex;
        align-items: center;
        justify-content: center;
        
        iframe {
          display: block;
          margin: 0 auto;
          width: 1120px;
          height: 630px;
        }
      }
    }

    .slick-next {
      right: 100px;
    }

    .slick-prev {
      left: 100px;
    }

</style>