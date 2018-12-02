<template>
  <div class="Newprodect">
    <div class="title">
      <span class="msg">新品专区</span>
      <i class="icon iconfont icon-icon-next"></i>
    </div>
    <div class="content">
      <div class="item" v-for="(pro,index)  in pros" :key="index">
        <span class="leftText">{{pro.leftText}}</span>
        <div class="imgCon">
          <img :src="pro.src" alt class="img">
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Newprodect",
  data() {
    return {
      pros: [
        { src: "./static/images/pc_1.png", leftText: "新品上市" },
        { src: "./static/images/pc_2.png", leftText: "满减专区" }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.Newprodect {
  .title {
    display: flex;
    justify-content: space-between;
    height: 2.08rem;
    border-bottom: 1px solid #e5e5e5;
    align-items: center;
    .msg {
      margin-left: 0.5rem;
    }
    .icon-icon-next {
      margin-right: 0.5rem;
    }
  }
  .content {
    display: flex;
    height: 6rem;
    .item {
      width: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      .leftText {
        font-size: 12px;
      }
      .imgCon {
        width: 60%;
        .img {
          width: 4.48rem;
          height: 3rem;
        }
      }
    }
  }
}
</style>
