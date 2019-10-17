<template>
  <div class="banner">
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide swiper-slide1">
          <img src="../../assets/img/gaogao_banner_01.png" alt />
        </div>
        <div class="swiper-slide swiper-slide2">
          <img src="../../assets/img/gaogao_banner_02.png" alt />
        </div>
      </div>
    </div>
    <div class="bannerAdv">
      <div class="bannerAdv_content w">
        <div class="bannerAdv_left fl">
          <a href="#">
            <i class="iconfont iconvolume_icon"></i>
            <span @mouseover="onMouseOver" @mouseout="onMouseOut">v2.8.9版本发布公告</span>
          </a>
        </div>
        <div class="bannerAdv_right fr">
          <a href="#">
            <i class="iconfont iconxinhao1"></i>
            <span @mouseover="onMouseOver" @mouseout="onMouseOut">我要买稿</span>
          </a>
          <a href="#">
            |
            <i class="iconfont iconyumao"></i>
            <span @mouseover="onMouseOver" @mouseout="onMouseOut">我要卖稿</span>
          </a>
          <a href="#">
            |
            <i class="iconfont iconi"></i>
            <span @mouseover="onMouseOver" @mouseout="onMouseOut">了解稿稿</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from "swiper";
import "swiper/css/swiper.min.css";
export default {
  name: "Banner",
  props: {
    msg: String
  },
  methods: {
    onMouseOver(params) {
      params.currentTarget.className = "underline";
      // console.log("鼠标移入", this);
    },
    onMouseOut(params) {
      params.currentTarget.className = "";
      // console.log("鼠标移出", this);
    },
    onClick() {
      console.log("点击事件");
    }
  },
  mounted() {
    var mySwiper = new Swiper(".swiper-container", {
      autoplay: true,
      loop: true
    });
  }
};
</script>

<style scoped lang="less">
.banner {
  padding-top: 67px;
  box-sizing: border-box;
  .swiper-container {
    // background: rgb(100, 161, 226);
    .swiper-slide1 {
      background-color: #333;
    }
    .swiper-slide2 {
      background-color: #64a1e2;
    }
  }
  .bannerAdv {
    background: rgba(0, 0, 0, 0.3);
    bottom: 0;
    z-index: 2;
    width: 100%;
    left: 0;
    position: relative;
    top: -50px;
    .bannerAdv_content {
      height: 50px;
      line-height: 50px;
      a {
        color: #fff;
        padding: 0 8px;
        float: left;
        span {
          &.underline {
            border-bottom: 1px solid #fff;
            padding-bottom: 1px;
          }
        }
        .iconfont {
          padding-right: 8px;
        }
      }
    }
  }
}
</style>
