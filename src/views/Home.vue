<template>
  <div>
    <div class="container">
      <NavBar />
      <Banner />
      <Collect />
      <Category />
      <Feed />
      <Rare />
    </div>
  </div>
</template>

<script>
// @ 引入组件
import "@/assets/css/index.css";
import "@/assets/font/iconfont.css";
import NavBar from "@/components/Home/NavBar.vue";
import Banner from "@/components/Home/Banner.vue";
import Collect from "@/components/Home/Collect.vue";
import Category from "@/components/Home/Category.vue";
import Feed from "@/components/Home/Feed.vue";
import Rare from "@/components/Home/Rare.vue";

export default {
  name: "home",
  components: {
    NavBar,
    Banner,
    Collect,
    Category,
    Feed,
    Rare
  }
};
</script>

<style scoped lang="less">
</style>
