<template>
  <div class="layouts-wrapper">
    <Header></Header>
    <div class="content">
      <slot/>
    </div>
    <Footer></Footer>
  </div>
</template>
<script setup lang="ts">
</script>

<style>
.layouts-wrapper {
  box-sizing: border-box;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background-color: #02041e;

  .content {
    box-sizing: border-box;
    width: 100%;
    height: calc(100vh - 120px);
    overflow-y: auto;
  }
}
</style>