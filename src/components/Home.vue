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

  export default {
    name: 'Home',
    components: {
      HeaderArea,
      ContentArea,
      FooterArea,
    },
  };
</script>

<style lang="scss">

</style>
