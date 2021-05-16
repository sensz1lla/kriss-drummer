<template>
  <Slide right>
    <a id="home" href="#home">
      <span>Home</span>
    </a>
    <a id="aboutMe" href="#aboutMe">
      <span>About Me</span>
    </a>
    <a id="portfolio" href="#portfolio">
      <span>Portfolio</span>
    </a>
    <a id="coversVideo" href="#coversVideo">
      <span>Covers Video</span>
    </a>
  </Slide>
</template>

<script>

  import { Slide } from 'vue-burger-menu'

  export default {
    components: {
      Slide
    }
  }

</script>

<style>

  .bm-burger-button {
      position: fixed;
      width: 40px;
      height: 30px;
      left: auto;
      right: 3.1% !important;
      top: 6.5%;
      cursor: pointer;
    }
    .bm-burger-bars {
      background-color: #fff;
    }
    .bm-burger-bars:nth-child(even) {
      width: 28px;
    }
    .bm-burger-bars:last-of-type {
      width: 18px;
    }
    .line-style {
      position: absolute;
      height: 2px;
      left: 0;
      right: 0;
    }
    .cross-style {
      position: absolute;
      top: 12px;
      right: 2px;
      cursor: pointer;
    }
    .bm-cross {
      background: #bdc3c7;
    }
    .bm-cross-button {
      height: 24px;
      width: 24px;
    }
    .bm-menu {
      height: 100%; /* 100% Full-height */
      width: 0; /* 0 width - change this with JavaScript */
      position: fixed; /* Stay in place */
      z-index: 1000; /* Stay on top */
      top: 0;
      left: 0;
      background-color: rgba(33,33,33, 0.8); /* Black*/
      backdrop-filter: blur(10px); /* This be the blur*/
      overflow-x: hidden; /* Disable horizontal scroll */
      padding-top: 60px; /* Place content 60px from the top */
      transition: 0.5s; /*0.5 second transition effect to slide in the sidenav*/
    }
 
    .bm-overlay {
      background: #0a0a0a;
    }
    .bm-item-list {
      color: #b8b7ad;
      margin-left: 10%;
      font-size: 20px;
    }
    .bm-item-list > * {
      display: flex;
      text-decoration: none;
      padding: 0.7em;
    }
    .bm-item-list > *:hover {
      color: #d14242;
    }
    .bm-item-list > * > span {
      margin-left: 10px;
      font-weight: 700;
      color: white;
    }

</style>