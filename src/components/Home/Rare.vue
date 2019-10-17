<template>
  <div class="rare w">
    <div class="rare_title">
      <span class="rare_title_txt fl">百里挑一</span>
    </div>
    <p>稿稿御用高端创作者社群，汇集平台最顶尖的创作者，俱乐部成员享受专属vip特权，高薪+特权 C位出道</p>
    <ul class="rare_category w">
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
.rare {
  background-color: #fff;
  margin-top: 20px;
  padding-top: 40px;
  p {
    margin-top: 15px;
    margin-bottom: 30px;
    text-align: left;
    padding-left: 15px;
    font-size: 16px;
    color: #666;
  }
  .rare_title {
    width: 98%;
    overflow: hidden;
    border-bottom: 1px solid #ddd;
    margin-top: 40px;
    margin: 0 15px;
    .rare_title_txt {
      text-align: left;
      font-size: 24px;
      display: inline-block;
      border-bottom: 3px solid #31a081;
      padding-bottom: 5px;
      // margin: 0 8px 0 4px;
    }
  }
  .rare_category {
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
