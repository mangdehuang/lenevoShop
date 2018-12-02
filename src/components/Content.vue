<template>
  <div class="Content">
    <Funcs></Funcs>
    <Mobile></Mobile>
    <Newprodects></Newprodects>
  </div>
</template>
    

<script>
import Funcs from "./Funcs";
import Mobile from "./Mobile";
import Newprodects from "./Newprodects";
export default {
  name: "Content",
  data() {
    return {};
  },
  components: {
    Funcs,
    Mobile,
    Newprodects
  }
};
</script>
<style lang="scss" scoped>
.Content {
  position: relative;
  top: 6rem;
}
</style>