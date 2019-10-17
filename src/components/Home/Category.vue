<template>
  <ul class="category w">
    <li class="cli1 fl">
      <div class="category_box">
        <img src="../../assets/img/category_01.png" alt />
      </div>
      <div class="category_info">商稿</div>
    </li>
    <li class="cli1 fl">
      <div class="category_box">
        <img src="../../assets/img/category_02.png" alt />
      </div>
      <div class="category_info">自媒体</div>
    </li>
    <li class="cli1 fl">
      <div class="category_box">
        <img src="../../assets/img/category_03.png" alt />
      </div>
      <div class="category_info">短视频</div>
    </li>
    <li class="cli1 fl">
      <div class="category_box">
        <img src="../../assets/img/category_04.png" alt />
      </div>
      <div class="category_info">专业稿件</div>
    </li>
    <li class="cli1 fl">
      <div class="category_box">
        <img src="../../assets/img/category_05.png" alt />
      </div>
      <div class="category_info">素材征集</div>
    </li>
  </ul>
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
.category {
  padding-top: 15px;
  overflow: hidden;
  .cli1 {
    width: 19.17%;
    background: #fff;
    display: inline-block;
    margin: 8px 4px 0;
    height: 160px;
    padding: 6px;
    border-radius: 5px;
    box-sizing: border-box;

    .category_box {
      position: relative;
      height: 94px;
      text-align: center;
      img {
        width: 56px;
        height: 56px;
        border-radius: 5px;
        margin-top: 24px;
      }
    }
    .category_info {
      width: 100%;
      padding: 12px 10px 0;
      position: relative;
      box-sizing: border-box;
    }
  }
}
</style>
