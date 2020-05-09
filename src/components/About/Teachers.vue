<template>
  <div class="teacher">
    <ul v-for="teacher in teachers" :key="teacher.id">
      <li class="clearfix">
        <div class="left fl">
          <img :src="teacher.img_url" alt="">
          <p class="name">{{teacher.name}}</p>
          <p class="position">{{teacher.position}}</p>
        </div>
        <div class="right fl">
          <p>{{teacher.intro}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
//在这里引入图片
import img from "@/assets/about/teacher.png"
export default {
  data:() => {
    return{
      teachers:[
        {
          id:1,
          img_url:img,
          name:"Ashok Khandelwal",
          position:"职业讲师",
          intro:"信息技术和管理硕士，软件工程高级文凭"
        },
        {
          id:2,
          img_url:img,
          name:"22222",
          position:"职业讲师",
          intro:"信息技术和管理硕士，软件工程高级文凭"
        },
        {
          id:3,
          img_url:img,
          name:"33333333",
          position:"职业讲师",
          intro:"信息技术和管理硕士，软件工程高级文凭"
        }
      ]
    }
  }
}
</script>

<style lang="less" scoped>
ul{
  margin-top: 16px;
}
li{
  background: url('~@/assets/about/teacher-bg.png') no-repeat;
  background-size: 100% 100%;
  overflow: hidden;
  display: flex;
  justify-content: center;
  width: 86%;
  align-items: center;
  margin: auto;
  border-radius: 6px;
  box-shadow: 0px 0px 7px #dedede;
  padding: 15px 10px;
  margin-bottom: 11px;
  .left{
    width: 45%;
    box-sizing: border-box;
    float: left;
    border-right: 2px solid #ececec;
        padding-right: 8px;
    img{
      width: 45%;
      margin: auto;
      display: block;
    }
    p{
      text-align: center;
      font-size: 14px;
      font-weight: bold;
      color: #454545;
    }
  }
  .right{
    width: 55%;
    box-sizing: border-box;
    float: left;
    font-size: 14px;
    p{
      padding-left: 8px;
    }
  }
}
</style>