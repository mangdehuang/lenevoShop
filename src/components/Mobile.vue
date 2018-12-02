<template>
  <div class="Mobile">
    <div class="title">
      <span class="msg">手机专享</span>
      <i class="icon iconfont icon-icon-next"></i>
    </div>
    <div class="pcs">
      <li class="item" v-for="(pc,index) in pcs" :key="index">
        <div class="pic">
          <img :src="pc.src">
        </div>
        <span class="price">{{'¥'+pc.price}}</span>
      </li>
    </div>
  </div>
</template>
<script>
export default {
  name: "Mobile",
  data() {
    return {
      pcs: [
        { src: "/static/images/mobile_1.png", price: "6499" },
        { src: "/static/images/mobile_2.png", price: "2788" },
        { src: "/static/images/mobile_3.png", price: "7245" },
        { src: "/static/images/mobile_4.png", price: "5666" }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.Mobile {
  .title {
    height: 2.08rem;
    border-bottom: 1px solid #e5e5e5;
    display: flex;
    align-items: center;
    justify-content: space-between;
    .msg {
      margin-left: 0.5rem;
    }
    .icon-icon-next {
      margin-right: 0.5rem;
    }
  }
  .pcs {
    border-bottom: 1px solid #e5e5e5;
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding-top: 0.56rem;
    height: 4.64rem;
    .item {
      display: flex;
      flex-direction: column;
      .pic {
        width: 3.36rem;
        height: 2.68rem;
        img {
          width: 100%;
          height: 100%;
        }
      }
      .price {
        text-align: center;
      }
    }
  }
}
</style>