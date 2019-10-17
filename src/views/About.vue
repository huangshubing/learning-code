<template>
  <div class="about">
    <h1>about页面</h1>
    <NavBar msg="msg" />
  </div>
</template>

<script>
// @ 引入helloworld组件
import NavBar from "@/components/Home/NavBar.vue";

export default {
  name: "home",
  components: {
    NavBar
  }
};
</script>