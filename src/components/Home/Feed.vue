<template>
  <div class="feed">
    <div class="feed_title w">
      <span class="feed_title_txt fl">供稿服务</span>
    </div>
    <ul class="feed_category w">
      <li class="cli1 fl">
        <div class="category_box">
          <img src="../../assets/img/feed_blank_01.png" alt />
        </div>
        <div class="category_info">
          <h3>媒体稿件</h3>
          <p>MEDIA</p>
        </div>
      </li>
      <li class="cli1 fl">
        <div class="category_box">
          <img src="../../assets/img/feed_blank_02.png" alt />
        </div>
        <div class="category_info">
          <h3>商业稿件</h3>
          <p>COMMERCIAL</p>
        </div>
      </li>
      <li class="cli1 fl">
        <div class="category_box">
          <img src="../../assets/img/feed_blank_03.png" alt />
        </div>
        <div class="category_info">
          <h3>专业稿件</h3>
          <p>PROFESSIONAL</p>
        </div>
      </li>
      <li class="cli1 fl">
        <div class="category_box">
          <img src="../../assets/img/feed_blank_04.png" alt />
        </div>
        <div class="category_info">
          <h3>图片图集</h3>
          <p>PICTURE</p>
        </div>
      </li>
      <li class="cli1 fl">
        <div class="category_box">
          <img src="../../assets/img/feed_blank_05.png" alt />
        </div>
        <div class="category_info">
          <h3>短视频</h3>
          <p>VIDEO</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Banner",
  props: {
    msg: String
  }
};
</script>

<style scoped lang="less">
.feed {
  background-color: #fff;
  margin-top: 20px;
  padding-top: 40px;
  .feed_title {
    width: 100%;
    overflow: hidden;
    .feed_title_txt {
      text-align: left;
      font-size: 24px;
      display: inline-block;
      border-bottom: 3px solid #31a081;
      padding-bottom: 5px;
      margin: 0 8px 0 4px;
    }
  }
  .feed_category {
    overflow: hidden;
    .cli1 {
      width: 19.17%;
      background: #f1f3f4;
      display: inline-block;
      margin: 8px 4px 0;
      height: 200px;
      padding: 6px;
      border-radius: 5px;
      box-sizing: border-box;
      .category_box {
        position: relative;
        height: 94px;
        text-align: center;
        overflow: hidden;
        img {
          transition: all 1s ease 0s;
          position: absolute;
          top: 0;
          left: 0;
        }
      }
      .category_info {
        padding: 30px 15px 0;
        text-align: left;
        h3 {
          font-weight: normal;
          font-size: 18px;
          padding-bottom: 5px;
        }
        p {
          font-size: 14px;
          color: #ddd;
          font-weight: 600;
        }
      }
    }
  }
}
</style>
