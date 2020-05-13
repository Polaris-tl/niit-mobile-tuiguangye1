<template>
  <div>
    <swiper :options="swiperOptions">
      <swiper-slide v-for="(item,index) in devData" :key="index">
        <div class="box">
          <img :src="item.bg_url" alt />
          <p class="year">{{item.year}}</p>
          <p class="detail">{{item.detail}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import bg1 from "@/assets/about/bg1.jpg";
import bg2 from "@/assets/about/bg2.png";
import bg3 from "@/assets/about/bg3.png";

export default {
  data() {
    return {
      swiperOptions: {
        spaceBetween: 44,
        slidesPerView: 2.5,
        freeMode: true
      },
      devData: [
        {
          year: "1997年",
          detail: "1997年，NIIT进入中国",
          bg_url: bg1
        },
        {
          year: "1998年",
          detail: "上海启动第一家直属学校",
          bg_url: bg2
        },
        {
          year: "2000年",
          detail: "重庆直属分校成立",
          bg_url: bg3
        },
        {
          year: "2001年",
          detail: "苏州、常州、海南、贵阳直属分校成立",
          bg_url: bg1
        },
        {
          year: "2003年",
          detail: "荣获《中国计算机报》授予的“年度最佳就业和最佳计算机学校”",
          bg_url: bg2
        },
        {
          year: "2004年",
          detail: "推出校企嵌入式合作模式，毕业学生对口就业",
          bg_url: bg3
        },
        {
          year: "2006年",
          detail: "NIIT与江苏省教育厅开始了正式合作",
          bg_url: bg1
        },
        {
          year: "2008年",
          detail: "推出BOD模式、PPP模式、公私合作模式",
          bg_url: bg2
        }
      ]
    };
  }
};
</script>

<style lang="less" scoped>
.box {
  border: 4px solid rgb(255, 255, 255);
  background-color: rgb(191, 191, 191);
  box-shadow: 0px 0px 8.64px 0.36px rgba(0, 15, 25, 0.3);
  height: 150px;
  text-align: center;
  position: relative;
  img {
    position: absolute;
    left: 0;
    top: 0;
    z-index: 0;
    width: 100%;
    height: 100%;
  }
  &::after {
    content: "";
    width: 15px;
    height: 30px;
    position: absolute;
    top: 0;
    bottom: 0;
    margin: auto;
    right: -34px;
    background: url("~@/assets/about/rightArrow.png") no-repeat;
    background-size: contain;
  }
  .year {
    margin-top: 30px;
    font-size: 16px;
    color: rgb(255, 235, 11);
    font-weight: bold;
    line-height: 1.2;
    text-shadow: 0px 0px 8.64px rgba(0, 15, 25, 0.3);
    position: relative;
    margin-bottom: 10px;
    &::after {
      content: "";
      width: 30px;
      height: 3px;
      background: #fff;
      position: absolute;
      left: 0;
      right: 0;
      bottom: -6px;
      margin: auto;
    }
  }
  .detail {
    font-size: 12px;
    color: rgba(255, 255, 255, 0.74);
    padding: 10px 6px 0 6px;
    position: relative;
  }
}
</style>