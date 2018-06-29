<template>
  <div class="layout">
    <Login id="login" v-if="loginNeed"></Login>
    <div class="container_first">
      <Header></Header>
      <div class="container_second">
        <Aside id="aside"></Aside>
        <Main id="main"></Main>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  .layout {
    width: 100vw;
    height: 100vh;
    background: #eee;
    // position: relative;

    #login {
      position: fixed;
      margin: auto;
      left: 0;
      right: 0;
      top: 0;
      bottom: 0;
    }

    .container_first {
      height: 100vh;
      display: flex;
      display: -webkit-flex;
      flex-direction: column;

      .container_second {
        height: 100%;
        // border: 1px solid red;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        margin: 8px 8px 8px 0;

        #aside {
          width: 19.5%;
          height: 100%;
        }
        #main {
          width: 79.5%;
          height: 100%;
        }
      }
    }
  }
  
</style>

<script>
  import Header from './components/Header'
  import Aside from './components/Aside'
  import Main from './components/Main'
  import Login from './components/Login'

  export default {
    data () {
      return {
        loginNeed: true
      }
    },
    components: {
      Header,
      Aside,
      Main,
      Login
    }
  };
</script>
