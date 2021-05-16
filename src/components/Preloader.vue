<template>
  <div class="preloader">
    <div class="preloader-logo">kriss_drummer</div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss">

  .preloader {
    position: fixed;
    top: 0;
    left: 0;
    background-color: #0a0a0a;
    color: #fff;
    width: 100%;
    height: 100%;
    z-index: 999;
    display: flex;
    justify-content: center;
    align-items: center;
    animation: slideFade .5s ease-in-out forwards;
    animation-delay: 1.5s;

    @keyframes slideFade {
        0% {
          transform: translateX(0);
        }
        100% {
          transform: translateX(100%);
        }
      }

    .preloader-logo {
      position: relative;
      font-size: 3rem;
      animation: zoom .5s ease-in-out forwards;
      transform: scale(1);
      overflow: hidden;

      @keyframes zoom {
        0% {
          transform: scale(1);
        }
        100% {
          transform: scale(1.2);
        }
      }

      &::before {
        position: absolute;
        content: '';
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: #fff;
        transform: translateX(-110%);
        animation: slide 1s ease-in-out forwards;
        animation-delay: .5s;
      }

      @keyframes slide {
        0% {
          transform: translateX(-110%);
        }
        
        100% {
          transform: translateX(0);
        }
      }
    }
  }

</style>