<template>
  <swiper :options="swiperOptions">
    <swiper-slide v-for="(item,index) in stuData" :key="index">
      <div class="hack">
        <div class="wrap">
          <div class="imgBox">
            <img :src="item.img_url" alt />
          </div>
          <p class="name">{{item.name}}</p>
          <p class="salary">
            月薪：
            <span>{{item.salary}}</span>
          </p>
          <p class="position">{{item.position}}</p>
          <p class="conpany">{{item.conpany}}</p>
        </div>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>
import img1 from '@/assets/employment/01.png';
import img2 from '@/assets/employment/02.png';
import img3 from '@/assets/employment/03.png';
import img4 from '@/assets/employment/04.png';
import img5 from '@/assets/employment/05.png';
import img6 from '@/assets/employment/06.png';
import img7 from '@/assets/employment/07.png';
import img8 from '@/assets/employment/08.png';
import img11 from '@/assets/employment/11.png';

export default {
  name: "Gaoxin",
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 2.5,
        autoplay: {delay:3000},
      },
      stuData: [
        {
          img_url:img1,
          name:"陈*",
          salary:9000,
          position:"前端工程师",
          conpany:"华***信科技信息有限公司"
        },
        {
          img_url:img2,
          name:"王*",
          salary:12000,
          position:"JAVA高级工程师",
          conpany:"金**泰科技有限公司"
        },
        {
          img_url:img3,
          name:"王*念",
          salary:11000,
          position:"运维工程师",
          conpany:"重庆电**寻科技有限公司"
        },
        {
          img_url:img4,
          name:"刘*能",
          salary:8500,
          position:"UI设计师",
          conpany:"重庆飞*画科技有限公司"
        },
        {
          img_url:img5,
          name:"周*",
          salary:11000,
          position:"JAVA工程师",
          conpany:"成都竹**染科技有限公司"
        },
        {
          img_url:img6,
          name:"肖*雅",
          salary:9000,
          position:"前端工程师",
          conpany:"重庆神**岳信息科技有限公司"
        },
        {
          img_url:img7,
          name:"陈*美",
          salary:10000,
          position:"UI设计师",
          conpany:"北京金**新科技有限公司"
        },
        {
          img_url:img8,
          name:"唐*磊",
          salary:12000,
          position:"嵌入式开发工程师",
          conpany:"重庆金**安科技有限公司"
        },
        {
          img_url:img11,
          name:"姜*",
          salary:10000,
          position:"游戏原画师",
          conpany:"亮**色科技有限公司"
        },

      ]
    };
  }
};
</script>

<style lang="less" scoped>
.hack {
  margin: 6px;
  .wrap {
    box-shadow: 0 0 6px #cacaca;
    border-radius: 2px;
    font-size: 12px;
    padding: 6px;
    color: #818181;
    .imgBox{
      height: 80px;
      width: 80px;
      border-radius: 100%;
      margin: auto;
      display: block;
      overflow: hidden;
      img {
        object-fit: fill;
      }
    }
    p{
      overflow: hidden;
      text-overflow: ellipsis;
      word-wrap:none;
      white-space: nowrap;
    }
    .name {
      text-align: center;
      font-weight: bold;
      margin: 4px 0 6px 0;
      font-size: 14px;
      color: #363636;
    }

    .salary {
      font-weight: bold;
      font-size: 12px;
      span {
        color: #ff984d;
      }
    }
    .position {
      font-size: 12px;
      text-indent: 10px;
      position: relative;
      &::before {
        content: "";
        width: 4px;
        height: 4px;
        background: #ff984d;
        border-radius: 100%;
        position: absolute;
        left: 0;
        top: 6px;
      }
    }
    .conpany {
      font-size: 12px;
      text-indent: 10px;
      position: relative;
      &::before {
        content: "";
        width: 4px;
        height: 4px;
        background: #ff984d;
        border-radius: 100%;
        position: absolute;
        left: 0;
        top: 6px;
      }
    }
  }
}
</style>