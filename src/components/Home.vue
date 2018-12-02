<template>
  <div>
    <Header></Header>
    <Content></Content>
    <Bottom></Bottom>
  </div>
</template>
<script>
import Header from "./Header.vue";
import Content from "./Content";
import Bottom from "./Bottom";
export default {
  name: "Home",
  components: {
    Header,
    Content,
    Bottom
  }
};
</script>
<style lang="scss" scoped>
</style>
    