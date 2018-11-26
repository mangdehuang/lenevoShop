<template>
  <div class="Header">
    <div class="title">
      <div class="search-scan">
        <i class="icon iconfont icon-icon-scan"></i>
      </div>
      <div class="search-input">
        <i class="search-btn icon iconfont icon-icon-search"></i>
        <input type="text" v-model="searchVal" class="search-input-ele">
      </div>
      <div class="message">
        <i class="icon iconfont icon-icon-messsage"></i>
      </div>
    </div>
    <div class="scroll">
      <img class="banner" :src="banner.src" alt>
    </div>
  </div>
</template>
<script>
export default {
  name: "Header",
  data() {
    return {
      searchVal: "搜索所有联想产品",
      banner: {
        src: "/static/images/banner.jpg"
      }
    };
  }
};
</script>
<style lang="scss" scoped>
@import "@/assets/style/global.scss";
.Header {
  color: #fff;
  position: relative;
  width: 100%;
  background: red;
  .title {
    height:1.2rem;
    background: #f39b15;
    display: flex;
    position: relative;
    z-index: 1;
    .icon.iconfont {
      font-size: 0.9rem;
    }
    .search-scan {
      flex: 1;
      @include center;
    }
    .search-input {
      flex: 3;
      position: relative;
      @include center();
      .search-btn {
        position: absolute;
        font-size: 1rem;
        left: .08rem;
      }
      .search-input-ele {
        border-radius: .16rem;
        color: #e8e8e8;
        text-align: center;
        background-color: #db8d14;
        background-color: transparent;
        justify-content: flex-start;
        margin-left: 0;
        height: 100%;
        width: 100%;
        filter: alpha(opacity=0); /*androd*/
        appearance: none; /*下拉框去掉右侧图标*/
        -moz-appearance: none;
        -webkit-appearance: none;
      }
    }
    .message {
      @include center;
      flex: 1;
    }
  }
  .scroll {
    position: absolute;
    z-index: 0;
    width: 100%;
    .banner {
      width: 100%;
      height: 6.32rem;
      background: red;
    }
  }
}
</style>
    