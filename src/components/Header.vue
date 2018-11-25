<template>
    <div class="Header">
        <div class="search-scan">
            <i class="icon iconfont icon-saoyisao"></i>
        </div>
        <div class="search-input" >
          <div class="search-btn"></div>
          <input type="text" v-model="searchVal">
        </div>
        <div class="message">
          <i class="icon iconfont icon-duihuakuang "></i>
        </div>
    </div>
</template>
<script>
export default {
  name: "Header",
  data() {
    return {
      searchVal: "搜索所有联想产品"
    };
  }
};
</script>
<style lang="scss" scoped>
@import "@/assets/style/global.scss";
.Header {
  background: red;
  .icon.iconfont {
    font-size: 1.666667rem;
    color: #fff;
  }
}
</style>
    