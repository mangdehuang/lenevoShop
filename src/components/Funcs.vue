<template>
  <div class="Funcs">
    <div class="content">
      <li class="item" v-for="(fun,index) in funs" :key="index">
        <img href class="pic" :src="fun.src">
        <span class="title">{{fun.name}}</span>
      </li>
    </div>
  </div>
</template>
<script>
export default {
  name: "Funcs",
  data() {
    return {
      funs: [
        { name: "新品", src: "/static/images/icon_news.png" },
        { name: "领券", src: "/static/images/icon_coupon.png" },
        { name: "伙伴", src: "/static/images/icon_partener.png" },
        { name: "客服", src: "/static/images/icon_customer.png" },
        { name: "物流", src: "/static/images/icon_logistical.png" }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.Funcs {
  display: flex;
  height: 3.2rem;
  background: #fff;
  position: relative;
  .content {
    display: flex;
    justify-content: space-around;
    width: 100%;
    border-bottom: 1px solid #e5e5e5;
    align-items: center;
    .item {
      display: flex;
      flex-direction: column;
      .pic {
        width: 1.6rem;
        height: 1.6rem;
      }
      .title {
        text-align: center;
        color: #9f9f9f;
      }
    }
  }
}
</style>