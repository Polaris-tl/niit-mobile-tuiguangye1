<template>
  <div class="teacher">
    <ul v-for="(teacher,index) in teachers" :key="index">
      <li class="clearfix">
        <div class="left fl">
          <img :src="teacher.img_url" alt />
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
import img1 from "@/assets/about/06/Ashok Khandelwal.png";
import img2 from "@/assets/about/06/BhushanParadkar.png";
import img3 from "@/assets/about/06/ManishKumarMalhan.png";
import img4 from "@/assets/about/06/Vishal.png";
import img5 from "@/assets/about/06/Akash.png";
import img6 from "@/assets/about/06/FaizalNujumudeen.png";
import img7 from "@/assets/about/06/Prashant.png";
export default {
  data: () => {
    return {
      teachers: [
        {
          img_url: img1,
          name: "Ashok Khandelwal",
          position: "职业讲师",
          intro: "信息技术和管理硕士，软件工程高级文凭"
        },
        {
          img_url: img2,
          name: "Bhushan Paradkar",
          position: "职业讲师",
          intro:
            "获得了计算机应用硕士学位，过去5年一直在教授.Net技术课程。"
        },
        {
          img_url: img3,
          name: "Manish Kumar Malhan",
          position: "职业讲师",
          intro:
            "工商管理硕士，英语应用硕士，软件工学高级学位。"
        },
        {
          img_url: img4,
          name: "Vishal",
          position: "职业讲师",
          intro: "计算机应用硕士，并获得了微软认证讲师（SCP和SCWCD）和Java认证"
        },
        {
          img_url: img5,
          name: "Akash",
          position: "职业讲师",
          intro: "信息技术硕士，SCJP和MCPD认证;在NIIT和淮阴工学院10年的经验"
        },
        {
          img_url: img6,
          name: "Faizal Nujumudeen",
          position: "职业讲师",
          intro:
            "计算机应用硕士,4年助理教授经验，2年PHP、web开发经验，熟悉核心PHP脚本、Java编程和Mysql。"
        },
        {
          img_url: img7,
          name: "Prashant",
          position: "职业讲师",
          intro:
            "一名工程师及软件培训师，过去3年半一直培训Java技术，希望教授更多不同技术。"
        }
      ]
    };
  }
};
</script>

<style lang="less" scoped>
ul {
  margin-top: 16px;
}
li {
  background: url("~@/assets/about/teacher-bg.png") no-repeat;
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
  .left {
    width: 45%;
    box-sizing: border-box;
    float: left;
    border-right: 2px solid #ececec;
    padding-right: 8px;
    img {
      width: 45%;
      margin: auto;
      display: block;
      border-radius: 50%;
      border: 2px #0eace2 solid;
    }
    p {
      text-align: center;
      font-size: 14px;
      font-weight: bold;
      color: #454545;
    }
  }
  .right {
    width: 55%;
    box-sizing: border-box;
    float: left;
    font-size: 14px;
    p {
      padding-left: 8px;
    }
  }
}
</style>