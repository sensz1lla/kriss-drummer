<template>
  <div id="portfolio" class="portfolio">
    <div class="portfolio-left"></div>
    <div class="portfolio-right">
      <h3 class="portfolio-title">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</h3>
      <div class="line"></div>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia impedit omnis modi velit esse culpa molestias consectetur inventore nulla vitae quidem commodi ea quae non ex nihil, et assumenda sint! Placeat saepe atque quasi veniam excepturi ipsa praesentium quo, sapiente blanditiis vero eos harum numquam voluptas ut quia alias eaque.</p>
    </div>
  </div>
</template>

<script>

  export default {
    //
  }

</script>

<style lang="scss">

  .portfolio{
    display: flex;
    height: 100vh;
    min-height: 700px;

    .portfolio-left {
      width: 50%;
      background-image: url('/img/kriss_image.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      background-position: 50%, 50%;
    }

    .portfolio-right {
      width: 50%;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;
      padding: 0 70px;

      .portfolio-title {
        margin-bottom: 20px;
      }

      p {
        font-weight: 300;
      }
    }
  }

</style>