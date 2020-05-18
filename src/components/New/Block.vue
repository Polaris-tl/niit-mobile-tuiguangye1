<template>
<div class="block">
  <div class="b1"></div>
  <div class="b2">
      <img v-lazy="img1" alt="" aos="flip-left" aos-duration="800" class="aos-init aos-animate">
      <img v-lazy="img2" alt="" aos="flip-right" aos-delay="100" aos-duration="800" class="aos-init aos-animate">
      <img v-lazy="img3" alt="" aos="flip-left" aos-delay="10" aos-duration="800" class="aos-init aos-animate">
  </div>
</div>
  
</template>


<script>

import img1 from "@/assets/index/block/01.png"
import img2 from "@/assets/index/block/02.png"
import img3 from "@/assets/index/block/03.png"
export default {
  data:() => {
    return{
      img1,img2,img3
    }
      
  }
}
</script>

<style lang="less" scoped>
.block{
  margin-top: 20px;
}
.b1{
  background: url("~@/assets/index/block/bg1-1.png");
    background-size: 100%;
    width: 100%;
    height: 87px;
}
.b2{
  background: url("~@/assets/index/block/bg1-2.png");
  background-size: 100% 100%;
    width: 100%;
    padding-top: 12px;
    padding-bottom: 55px;
    height: auto;
    img{
          width: 77%;
    margin-top: 10px;
    margin: 10px auto;
    display: block;
    }
}
</style>