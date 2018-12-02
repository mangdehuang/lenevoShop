<template>
  <div class="Bottom">
    <li :class="['item',{'red':checkbtn == index}]" v-for="(btn,index) in btns" :key="index">
      <i class="icon iconfont" :class="[btn.class,]"></i>
      <span class="msg">{{btn.name}}</span>
    </li>
  </div>
</template>
<script>
export default {
  name: "Bottom",
  data() {
    return {
      checkbtn: 0,
      btns: [
        { name: "首页", class: "icon-home" },
        { name: "分类", class: "icon-icon-type" },
        { name: "购物车", class: "icon-shopcart" },
        { name: "我的", class: "icon-mine" }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.Bottom {
  height: 1.96rem;
  display: flex;
  background: #e2e2e2;
  justify-content: space-around;
  align-items: center;
  position: fixed;
  bottom: 0;
  width: 100%;
  .item {
    display: flex;
    flex-direction: column;
    justify-content: center;
    .icon {
      width: 0.88rem;
      height: 0.88rem;
      text-align: center;
    }
    .msg {
      text-align: center;
      font-size: 0.44rem;
    }
  }
  .red {
    color: red;
  }
}
</style>
