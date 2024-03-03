<script setup lang="ts">
</script>

<template>
  <div class="footer">
    <div class="content-wrapper">
      <div class="item">
        <img src="../../assets/image/logo-ga.png" alt="" style="width: 20px;margin-right: 5px;">
        <a href="https://beian.mps.gov.cn/#/query/webSearch?recordcode=51010602002116" target="_blank">
          川公网安备51010602002116号
        </a>
      </div>
      <div class="item">
        <a href="https://beian.miit.gov.cn/" target="_blank" style="margin-left: 10px">
          蜀ICP备2024050890号-1
        </a>
      </div>
    </div>
    <div class="privacy-policy">
      <NuxtLink to="/privacyPolicy" class="text">
        隐私政策
      </NuxtLink>
      <div class="line"></div>
      <NuxtLink to="/support" class="text">
        技术支持
      </NuxtLink>
      <div class="line"></div>
      <span class="text">联系方式: 1761617270@qq.com</span>
    </div>
  </div>
</template>

<style scoped lang="less">
.footer {
  box-sizing: border-box;
  height: 60px;
  display: flex;
  justify-content: space-around;
  align-items: center;

  .content-wrapper {
    box-sizing: border-box;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    .item {
      display: flex;
      justify-content: center;
      align-items: center;

      img {
        width: 45px;
      }

      a {
        color: #b7bfd7;
        text-decoration: none;
        font-size: 13px;

        &:hover {
          color: whitesmoke;
        }
      }
    }

  }

  .privacy-policy {
    display: flex;

    .line {
      width: 2px;
      height: 20px;
      background-color: whitesmoke;
      margin: 0 15px;
    }

    .text {
      color: whitesmoke;
      text-decoration: none;
      font-size: 13px;
      cursor: pointer;
    }
  }
}
</style>