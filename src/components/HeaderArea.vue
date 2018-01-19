<template>
  <nav id="main-nav">
    <div class="fork-me">
      <a href="https://github.com/SakilaWAW"><img style="position: absolute; top: 0; left: 0; border: 0;"
                                            src="https://camo.githubusercontent.com/82b228a3648bf44fc1163ef44c62fcc60081495e/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f6769746875622f726962626f6e732f666f726b6d655f6c6566745f7265645f6161303030302e706e67"
                                            alt="Fork me on GitHub"
                                            data-canonical-src="https://s3.amazonaws.com/github/ribbons/forkme_left_red_aa0000.png"></a>
    </div>
    <ul id='link-lis'>
      <li><a href="">PORTFOLIO</a></li>
      <li><a href="">ABOUT</a></li>
      <li><img id='site-logo' alt="snake-logo" :src="logoSrcEntity"></li>
      <li><a href="">BLOG</a></li>
      <li><a href="">GET IN TOUCH</a></li>
    </ul>
    <div id="nav-decorator">
      <div class="decorate-line"></div>
      <div class="decorate-triangle"></div>
      <div class="decorate-line"></div>
    </div>
  </nav>
</template>

<script>
  const logo = require('../assets/logo.png');

  export default {
    name: 'header-area',
    data() {
      return {
        logoSrcEntity: logo,
      };
    },
  };
</script>

<style lang="scss" scoped>
  $navPrimary: #353535;

  #main-nav {
    background: $navPrimary;
    height: 0.95rem;
    font-size: 0;
    #link-lis {
      margin: 0 auto;
      height: 0.9rem;
      display: flex;
      align-items: center;
      justify-content: center;
      padding-top: 0.05rem;
      li {
        a {
          text-decoration: none;
          color: whitesmoke;
          font-size: 0.15rem;
          font-weight: 700;
          line-height: 1.5;
          margin: 0 0.2rem;
        }
        img {
          /*微调位置将logo置于中间*/
          position: relative;
          left: 0.035rem;
          margin: 0 0.25rem;
          height: 0.6rem;
          width: 0.6rem;
        }
      }
    }
    #nav-decorator {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      height: 0.3rem;
      .decorate-line {
        flex-grow: 1;
        height: 0.3rem;
        display: inline-block;
        position: relative;
        margin: 0 0.3rem;
        &::before {
          position: absolute;
          content: "";
          width: 100%;
          height: 0.02rem;
          background: #ECECEC;
          top: 0.15rem;
        }
      }
      .decorate-triangle {
        height: 0.6rem;
        width: 1.15rem;
        display: inline-block;
        box-sizing: border-box;
        border-top: solid 0.3rem $navPrimary;
        border-right: solid 0.575rem transparent;
        border-bottom: solid 0.3rem transparent;
        border-left: solid 0.575rem transparent;
      }
    }
  }
</style>
