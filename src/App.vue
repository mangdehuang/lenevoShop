<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
var html = document.documentElement;
html.style.fontSize = window.screen.width / 15 + "px";
export default {
  name: "App"
};
</script>

<style lang='scss'>
@import "assets/icon/iconfont.css";
@import "assets/style/global.scss";
</style>
