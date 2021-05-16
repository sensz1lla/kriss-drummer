<template>
  <header class="container-fluid">
    <div class="wrapper">
      <div class="header-logo">
        <a href="/" class="logo"><span>kriss_</span>drummer</a>
      </div>
      <Menu/>
    </div>
  </header>
</template>

<script>

  import Menu from '@/components/Menu.vue'

  export default {
    name: 'Header',
    props: {
      msg: String
    },
    components: {
      Menu
    }
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  
  header {
    .wrapper {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 50px 50px 0;
      position: absolute;
      width: 100%;
      top: 0;
      left: 0;
      z-index: 1;

      .header-logo {
        .logo {
          display: inline-block;
          color: #fff;
          font-size: 2.4rem;
          font-weight: 300;
          text-decoration: none;

          span {
            color: #d14242;
            font-weight: 700;
          }
        }
      }
    }
  }

</style>
