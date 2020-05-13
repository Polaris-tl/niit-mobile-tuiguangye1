<template>
  <ul>
    <li v-for="(ques,index) in questions" v-bind:key="index">
      <p>{{ques}}</p>
      <a class="button" href="http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn">点击咨询</a>
    </li>
  </ul>
</template>

<script>
export default {
    data(){
        return{
            questions:[
                "学费多少？可以分期吗？",
                "没有基础可以学会吗?",
                "你们学了后能拿什么文凭",
                "贫困补助申请有什么条件?",
                "你们都有哪些专业?",
                "有没有电竞专业?",
                "毕业后学校会不会分配工作?",
                "毕业以后可以报考公务员吗？"
            ]
        }
    }
}
</script>

<style lang="less" scoped>
ul {
  width: 80%;
  margin: auto;
  padding: 16px;
  border-radius: 4px;
  box-shadow: 0 0 5px #d0d0d0;
  li {
    overflow: hidden;
    font-size: 14px;
    border-bottom: 1px dashed #b1b1b1;
    padding: 0 5px;
    padding-bottom: 5px;
        margin: 10px 0;
    p {
      &:first-child {
        box-sizing: border-box;
        float: left;
        width: 70%;
        line-height: 30px;
      }
    }
    a {
      float: left;
      display: block;
      box-sizing: border-box;
      width: 30%;
      background: #2fa0ff;
      border-radius: 2px;
      height: 25px;
      line-height: 25px;
      color: #fff;
      text-align: center;
      box-shadow: 2px 3px 0px #3b7fb9db;
    }
  }
}
</style>