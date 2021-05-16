<template>
  <div id="home" class="main">
    <Preloader/>
    <Header/>
    <div class="hero">
      <video class="hero-video" width="400" height="300" muted autoplay loop>
        <source src="videos/kriss_video.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
      </video>
      <div class="hero-content">
        <transition enter-active-class="animated animate__fadeInLeft" mode="out-in">
          <h1 class="hero-title">Kristina Rybalchenko</h1>
        </transition>
        <p>YouTube channel/session drummer/drum teacher</p>
        <a href="#" class="hero-btn">Go to</a>
      </div>
    </div>
    <AboutMe/>
    <Portfolio/>
    <SliderVideo/>
    <Footer/>
  </div>
</template>

<script>

  // @ is an alias to /src
  import Preloader from '@/components/Preloader.vue'
  import Header from '@/components/Header.vue'
  import AboutMe from '@/components/AboutMe.vue'
  import Portfolio from '@/components/Portfolio.vue'
  import SliderVideo from '@/components/SliderVideo.vue'
  import Footer from '@/components/Footer.vue'

  export default {
    name: 'Main',
    components: {
      Preloader,
      Header,
      AboutMe,
      Portfolio,
      SliderVideo,
      Footer
    }
  }

</script>

<style lang="scss">

  .hero {
    position: relative;
    width: 100%;
    height: 100vh;
    left: 0;
    top: 0;
    //z-index: -1;

    .hero-video {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    &::before {
      content: '';
      position: absolute;
      width: 100%;
      height: 100%;
      min-height: 100vh;
      left: 0;
      top: 0;
      z-index: 0;
      background-color: #000;
      opacity: .4;
    }

    .hero-content {
      position: absolute;
      top: 20%;
      bottom: 0;
      width: 100%;
      padding: 120px 40px 75px 6.6%;
      text-align: left;

      .hero-title {
        font-size: 4.5rem;
        margin-bottom: 15px;
      }

      p {
        font-size: 1.1rem;
        font-weight: 300;
        margin-bottom: 50px;
      }

      .hero-btn {
        display: inline-block;
        padding: 12px 40px;
        border: 2px solid #d14242;
        color: #d14242;
        text-align: center;
        transition: .3s ease;
        text-decoration: none;

        &:hover {
          background-color: #d14242;
          color: #fff;
        }
      }
    }
  }

</style>