<template>
  <div class="head-bar">
    <nav id="nav-bar">
      <div class="logo">Logo</div>
      <ul class="title-href">
        <li>标签1</li>
        <li>标签2</li>
        <li>标签3</li>
        <li>标签4</li>
      </ul>
    </nav>
  </div>
</template>

<script>
  export default {
    name: 'header-area',
  };
</script>

<style lang="scss" scoped>
#nav-bar {
  display: flex;
  flex-direction: row;
}
</style>
