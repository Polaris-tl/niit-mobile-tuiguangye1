<template>
  <p>
    <a :href="url">了解更多>></a>
  </p>
</template>

<script>
export default {
  props:{
    url:{
      type:String,
      default:'http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn'
    }
  }
}
</script>>

<style lang="less" scoped>
  p{
    background: #23c7ff;
    width: 117px;
    height: 30px;
    text-align: center;
    line-height: 30px;
    font-size: 14px;
    border-radius: 100px;
    box-shadow: 2px 3px 1px rgba(62, 62, 62, 0.4);
    margin: auto;
    a{
      color: #fff;
      text-shadow: 0px 0px 8.64px rgba(0, 15, 25, 0.3);
    }
  }
</style>