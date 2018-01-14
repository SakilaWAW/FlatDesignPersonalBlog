<template>
  <div class="head-bar" :style="bannerBackground">
    <div id="mask"></div>
    <nav id="nav-bar">
      <div class="logo"><a href="#">T<>T</a></div>
      <ul class="title-href">
        <li><a href="#">朱雀三生</a></li>
        <li><a href="#">玄阳</a></li>
        <li><a href="#">近水楼台先得月</a></li>
        <li><a href="#">逻辑</a></li>
      </ul>
    </nav>
    <div class="banner">
      <div class="welcome-block">
        <span class="first-title">SakilaWAW</span>
        <span class="second-title">Talk is Cheap. Show me the code.</span>
        <span class="third-title">Never Give up.</span>
        <button>Now about me</button>
      </div>
    </div>
  </div>
</template>

<script>
  const bannerImg = require('../assets/banner_rain.jpg');

  export default {
    name: 'header-area',
    data() {
      return {
        bannerBackground: {
          backgroundImage: `url( ${bannerImg} )`,
          backgroundRepeat: 'no-repeat',
          backgroundSize: 'cover',
        },
      };
    },
  };
</script>

<style lang="scss" scoped>
  #mask {
    position: absolute;
    height: 10rem;
    width: 100%;
    background: rgba(0,0,0,0.2);
  }
  #nav-bar {
    position: relative;
    font-size: 0;
    display: block;
    background: transparent;
    height: 0.4rem;
    .logo {
      display: inline-block;
      font-size: 0.3rem;
      margin-left: 0.1rem;
      height: 0.4rem;
      line-height: 0.4rem;
    }
    .title-href {
      position: absolute;
      right: 0.1rem;
      top: 0;
      display: flex;
      align-items: center;
      font-size: 0.2rem;
      li {
        margin: 0 0.1rem;
        display: inline-block;
      }
    }
    a {
      text-decoration: none;
      color: white;
      display: inline-block;
      line-height: 0.4rem;
      height: 0.4rem;
    }
  }
  .banner {
    height: 10rem;
    width: 100%;
    .welcome-block {
      margin: 0 auto;
      width: 4rem;
      height: 4rem;
      position: relative;
      top: 5rem;
      transform: translateY(-50%);
      text-align: center;
      .first-title {
        font-size: 0.4rem;
        line-height: 1.0rem;
        border-bottom: 3px solid black;
        display: block;
      }
      .second-title {
        font-size: 0.2rem;
        line-height: 0.4rem;
        display: block;
      }
      .third-title {
        font-size: 0.2rem;
        line-height: 0.35rem;
        margin-bottom: 0.2rem;
        display: block;
      }
      button {
        border: none;
        background: #999;
        line-height: 0.4rem;
        height: 0.4rem;
        width: 1.2rem;
        font-weight: bold;
      }
    }
  }
</style>
