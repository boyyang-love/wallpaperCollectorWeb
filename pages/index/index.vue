<script setup lang="ts">
useHead({
  title: 'wallpaperCollector',
  meta: [
    {name: 'description', content: '桌面壁纸软件'},
    {name: 'description', content: 'macos壁纸软件'},
    {name: 'description', content: '电脑壁纸'},
    {name: 'description', content: '个性化壁纸'},
    {name: 'description', content: '壁纸管理'},
    {name: 'description', content: '个性化壁纸管理软件'},
    {name: 'description', content: '壁纸'},
  ],
})

const downloadApp = () => {
  window.open('https://apps.apple.com/app/wallpapercollector/id6476251931', '__blank')
}
</script>

<template>
  <div class="home">
    <div class="container">
      <div class="title">
        <span class="text">打造属于自己的个人壁纸软件</span>
        <span class="text">只收藏自己喜欢的精美壁纸</span>

        <div class="download-btn">
          <div class="btn" @click="downloadApp">前往下载</div>
        </div>
      </div>
      <div class="btns-wrapper" v-if="false">
        <div class="btn active">轮播展示</div>
        <div class="btn">图片列表</div>
        <div class="btn">壁纸收藏</div>
      </div>


      <div class="content-wrapper">
        <div class="video">
          <video
              autoplay
              loop
              src="../../assets/video/软件介绍.mp4"
              controls
              width="100%"
              height="100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="less">

.home {
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  overflow-y: auto;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  .title {
    width: 100%;
    height: 700px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    position: relative;

    .text {
      color: whitesmoke;
      font-size: 45px;
    }

    .download-btn {
      position: absolute;
      bottom: 50px;

      .btn {
        padding: 10px 20px;
        border: 1px solid whitesmoke;
        color: whitesmoke;
        font-weight: bold;
        border-radius: 5px;
        cursor: pointer;
      }
    }
  }

  .btns-wrapper {
    box-sizing: border-box;
    display: flex;
    justify-content: space-around;
    border: 2px solid whitesmoke;
    margin-top: 200px;
    border-radius: 20px;
    overflow: hidden;

    .btn {
      box-sizing: border-box;
      width: 100%;
      height: 100%;
      color: whitesmoke;
      font-weight: bold;
      padding: 10px 30px;
      border-radius: 20px;
      cursor: pointer;
    }

    .active {
      background-color: #e84a5f;
    }
  }

  .content-wrapper {
    box-sizing: border-box;
    margin-top: 80px;
    width: 65%;
    aspect-ratio: 3/2;
    border-radius: 20px;


    .video {
      box-sizing: border-box;
      display: flex;
      justify-content: center;
      align-items: center;

      video {
        border: 2px solid whitesmoke;
        border-radius: 20px;
        object-fit: cover;
      }
    }
  }
}
</style>