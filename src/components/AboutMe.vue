<template>
  <div id="aboutMe" class="about-me">
    <div class="about-me-left">
      <transition enter-active-class="animate__fadeInLeft" mode="out-in">
        <h3 class="about-me-title">Artist: Paist cymbals, Leonty drum sticks, Fat custom drums</h3>
      </transition>
      <!-- <h3 class="about-me-title">Artist: Paist cymbals, Leonty drum sticks, Fat custom drums</h3> -->
      <div class="line"></div>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Pariatur eveniet, non nostrum quisquam placeat quis
        magnam! Beatae nihil nam consectetur labore earum! Eaque nihil animi atque magnam velit. Quisquam, laboriosam?
      </p>
    </div>
    <div class="about-me-right"></div>
  </div>
</template>

<script>

  export default {
    // name: 'about-me',
    // data () {
    //   return {
    //     show: false
    //   }
    // }
  }

</script>

<style lang="scss">

  .about-me {
    display: flex;
    height: 100vh;
    min-height: 700px;

    .about-me-left {
      width: 50%;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;
      padding: 0 70px;

      .about-me-title {
        margin-bottom: 20px;
      }

      p {
        font-weight: 300;
      }
    }

    .about-me-right {
      width: 50%;
      background-image: url('/img/kriss_photo.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      background-position: 50%, 50%;
    }
  }

</style>