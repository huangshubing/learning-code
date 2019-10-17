<template>
  <div class="gaogao-nav">
    <div class="gg-home-navbar w">
      <div class="gg-home-navbar-logo fl">
        <a href="#">
          <img src="../../assets/img/gaogao_logo.png" alt />
        </a>
      </div>
      <div class="gg-home-navbar-nav">
        <ul>
          <li class="act">
            <a href="#">首页</a>
          </li>
          <li @mouseover="onMouseOver" @mouseout="onMouseOut">
            <a href="#">征稿令</a>
          </li>
          <li @mouseover="onMouseOver" @mouseout="onMouseOut">
            <a href="#">供稿服务</a>
          </li>
          <li @mouseover="onMouseOver" @mouseout="onMouseOut">
            <a href="#">
              <img src="../../assets/img/gaogao_nav_01.png" alt />
              稿稿社区
            </a>
          </li>
        </ul>
      </div>
      <div class="gg-home-navbar-btn fr">
        <a href="#" class="fl" @click="onClick">登录</a>
        <a href="#" class="fr" @click="onClick">注册</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    msg: String
  },
  methods: {
    onMouseOver(params) {
      params.currentTarget.className = "act";
      // console.log("鼠标移入", this);
    },
    onMouseOut(params) {
      params.currentTarget.className = "";
      // console.log("鼠标移出", this);
    },
    onClick() {
      console.log("点击事件");
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.gaogao-nav {
  width: 100%;
  height: 67px;
  background-color: #fff;
  position: fixed;
  top: 0;
  z-index: 20;
  .gg-home-navbar {
    background-color: #fff;
    display: flex;
    .gg-home-navbar-logo {
      padding: 17px 0;
      padding-right: 40px;
      a {
        width: 100%;
        height: 100%;
      }
      img {
        width: 90px;
        height: 30px;
      }
    }
    .gg-home-navbar-nav {
      height: 67px;
      flex: 1;
      ul {
        li {
          float: left;
          margin-right: 5px;
          border-top: solid 3px #fff;
          border-left: 1px solid #fff;
          border-right: 1px solid #fff;
          box-sizing: border-box;
          &.act {
            border-top: solid 3px #31a081;
            border-left: 1px solid #eee;
            border-right: 1px solid #eee;
          }
          a {
            padding: 0 12px;
            line-height: 64px;
            color: #333;
            box-sizing: border-box;
          }
        }
      }
    }
    .gg-home-navbar-btn {
      width: 130px;
      a {
        width: 50px;
        height: 30px;
        line-height: 30px;
        color: #666;
        border: 1px solid #666;
        border-radius: 5px;
        margin-top: 17px;
      }
    }
  }
}
</style>
