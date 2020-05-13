<template>
  <div class="section">
    <div class="head">
      <p>{{title}}</p>
      <a :href="url" >更多>></a>
    </div>
    <div style="background:#fafafa;padding: 18px 0;">
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  name:"Section",
  props:{
    title: String,
    url: {
      type:String,
      default:'http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn'
      },
  }
}
</script>

<style lang="less" scoped>
.section{
  padding: 20px 0 10px 0;
  .head{
    position: relative;
    font-size: 20px;
    font-family: "Microsoft YaHei";
    color: rgb(83, 83, 83);
    font-weight: bold;
    line-height: 1.2;
    text-align: center;
    padding-bottom: 23px;
    border-bottom: 2px solid #f3f3f3;
    margin-bottom: 15px;
    a{
      font-size: 12px;
      position: absolute;
      right: 2%;
      top: 0;
      bottom: 0;
      margin: auto;
      height: 10px;
      line-height: 10px;
      font-weight: normal;
      color: #444444;
    }
    p::after{
      content: '';
      width: 50px;
      height: 3px;
      background-color: #0d87fc;
      position: absolute;
      bottom: 12px;
      right: 0;
      left: 0;
      box-shadow: 0px 0px 4.85px 0.15px rgba(0, 15, 25, 0.29);
      margin: auto;
    }
  }
}
</style>