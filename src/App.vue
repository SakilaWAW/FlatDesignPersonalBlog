<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
  import 'reset-css';

  export default {
    name: 'app',
  };
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Open+Sans');
  html {
    font-family: "Open Sans",arial,x-locale-body,"Microsoft YaHei","黑体","宋体",sans-serif;
    font-size: 100px;
  }
</style>
