<template>
  <div class="more" :class="{reverse: !isBoxCollapse}">
    <img src="@/assets/about/downArrow.png" alt="" >
  </div>
</template>

<script>
export default {
  props:{
    isBoxCollapse:{
      type:Boolean,
      default:true
    }
  }
}
</script>

<style lang="less" scoped>
.more{
  width: 100%;
  height: 40px;
  position: absolute;
  bottom: 7px;
  
  img{
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    margin: auto;
    animation: down 0.6s linear infinite alternate;
    width: 23px;
  }
}
.reverse{
    transform: rotateZ(180deg);
  }
@keyframes down {
  to {
    transform: translate3d(0, -6px, 0);
  }
}
</style>