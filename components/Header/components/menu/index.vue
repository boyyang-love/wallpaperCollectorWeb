<script setup lang="ts">

</script>

<template>
  <div class="menu-wrapper">
    <div class="left-name">
      <NuxtLink to="/" class="text">
        wallpaperCollector
      </NuxtLink>
    </div>
  </div>
</template>

<style scoped lang="less">
.menu-wrapper {
  padding: 10px;
  display: flex;


  .left-name {
    .text {
      color: whitesmoke;
      font-style: italic;
      font-size: 22px;
      font-weight: bolder;
      display: flex;
      text-decoration: none;
      cursor: pointer;
    }
  }
}
</style>