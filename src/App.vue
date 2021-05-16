<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>

  export default {
    
  }

</script>

<style lang="scss">

  @import "~bootstrap/scss/bootstrap";
  //@import "~font-awesome/css/font-awesome.min.css";
  @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700;900&display=swap');

  body {
    background-color: #0a0a0a;
    color: #fff;
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 1px;
    font-family: 'Lato', sans-serif;
  }

  .line {
    width: 200px;
    max-width: 100%;
    height: 3px;
    background-color: #d14242;
    margin: 0 auto 20px 0;
  }

</style>