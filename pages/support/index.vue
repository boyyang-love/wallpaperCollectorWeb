<script setup lang="ts">

</script>

<template>
  <div class="support">
    <div class="title">
      <span class="title-text">
        wallpaperCollector App Tech Support
      </span>
    </div>
    <div class="content">
      <p class="content-title">
        <span>软件使用视频</span>
      </p>
      <div class="video-wrapper">
        <video
            autoplay
            loop
            src="../../assets/video/软件介绍.mp4"
            controls
        ></video>
      </div>
      <div class="desc">
        <ul>
          <li>下载软件后由于没有图片，所以用户需要自己导入本地壁纸</li>
          <li>导入壁纸后，最近导入地最多12张壁纸将进行轮播展示</li>
          <li>首页有3个按钮分别是 设置当前图片为桌面壁纸 添加新地图片壁纸 列表展示所有壁纸</li>
          <li>进入壁纸列表后，可以对图片的基本信息进行修改，加入收藏等相关操作</li>
        </ul>
      </div>
      <p class="content-title">
        <span>首页</span>
      </p>
      <div class="img-wrapper">
        <img src="../../assets/image/m_首页截图.png" alt="wallpaperCollector">
      </div>
      <p class="content-title">
        <span>壁纸列表</span>
      </p>
      <div class="img-wrapper">
        <img src="../../assets/image/m_列表页截图.png" alt="wallpaperCollector">
      </div>
      <p class="content-title">
        <span>收藏列表</span>
      </p>
      <div class="img-wrapper">
        <img src="../../assets/image/m_收藏页截图.png" alt="wallpaperCollector">
      </div>
    </div>
    <div class="bottom">
      <span>Getting Support:</span>
      <span>mail: 1761617270@qq.com </span>
    </div>
  </div>
</template>

<style scoped lang="less">
.support {
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  padding: 20px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  overflow-y: auto;

  .title {
    text-align: center;
    font-size: 24px;
    color: whitesmoke;
    font-weight: bold;
    margin-bottom: 50px;

    .title-text {
      padding: 10px;
      border-bottom: 2px solid white;
    }
  }

  .content {
    box-sizing: border-box;
    width: 100%;


    .content-title {
      text-align: center;
      color: whitesmoke;
      font-size: 16px;
      margin-bottom: 50px;

      span {
        position: relative;

        &::before {
          content: "";
          width: 100%;
          height: 5px;
          position: absolute;
          bottom: -10px;
          background-color: whitesmoke;
        }
      }


    }

    .video-wrapper,
    .img-wrapper {
      display: flex;
      justify-content: center;
      height: 400px;

      video, img {
        height: 100%;
      }
    }

    .desc{
      display: flex;
      justify-content: center;

      ul {
        display: flex;
        justify-content: flex-start;
        flex-direction: column;

        li {
          color: whitesmoke;
        }
      }
    }
  }

  .bottom {
    color: whitesmoke;
    text-align: center;
    font-size: 20px;
    display: flex;
    flex-direction: column;
    margin-top: 50px;
  }
}
</style>