<template>
  <div id="app">
    <public-header></public-header>
    <div class="container-fluid">
      <div class="row">
        <public-sidebar></public-sidebar>
        <content-list></content-list>
      </div>
    </div>
  </div>
</template>

<script>
// 引入bootstrap.css文件
import "../node_modules/bootstrap/dist/css/bootstrap.css";
// 引入index.css
import "./style/index.css";

import header from "./components/common/public_header.vue";
import sidebar from "./components/common/public_sidebar.vue";
import contentList from "./components/common/content_list.vue";

export default {
  name: "app",
  components: {
    "public-header": header,
    "public-sidebar": sidebar,
    "content-list": contentList
  }
};
</script>

<style>
</style>
