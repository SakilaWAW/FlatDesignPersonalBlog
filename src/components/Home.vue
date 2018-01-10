<template>
  <div>
    <headerArea></headerArea>
    <contentArea></contentArea>
    <footerArea></footerArea>
  </div>
</template>

<script>
  import HeaderArea from './HeaderArea';
  import ContentArea from './ContentArea';
  import FooterArea from './FooterArea';

  require('normalize.css');

  export default {
    name: 'Home',
    components: {
      HeaderArea,
      ContentArea,
      FooterArea,
    },
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
