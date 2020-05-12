<template>
  <swiper :options="swiperOptions">
    <swiper-slide v-for="(item,index) in stuData" :key="index">
      <div class="hack">
        <div class="wrap">
          <img :src="item.img_url" alt />
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
import img1 from '@/assets/employment/04.png';

export default {
  name: "Gaoxin",
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 2.5
      },
      stuData: [
        {
          img_url:img1,
          name:"陈亮",
          salary:8000,
          position:"前端切图仔",
          conpany:"公司：华清佳信"
        },
        {
          img_url:img1,
          name:"王健",
          salary:7000,
          position:"前端切图仔",
          conpany:"零起点科技"
        },
        {
          img_url:img1,
          name:"王思壹",
          salary:7000,
          position:"前端切图仔",
          conpany:"金网安泰"
        },
        {
          img_url:img1,
          name:"彭磊",
          salary:7000,
          position:"前端切图仔",
          conpany:"视腾信息"
        },
        {
          img_url:img1,
          name:"周*",
          salary:7000,
          position:"前端切图仔",
          conpany:"专业：JAVA精英班"
        },
        {
          img_url:img1,
          name:"肖*雅",
          salary:7000,
          position:"前端切图仔",
          conpany:"WEB精英班"
        },
        {
          img_url:img1,
          name:"陈亮",
          salary:7000,
          position:"前端切图仔",
          conpany:"金网安泰"
        },
        {
          img_url:img1,
          name:"陈亮",
          salary:7000,
          position:"前端切图仔",
          conpany:"金网安泰"
        },
        {
          img_url:img1,
          name:"陈亮",
          salary:7000,
          position:"前端切图仔",
          conpany:"金网安泰"
        },

      ]
    };
  }
};
</script>

<style lang="less" scoped>
.hack {
  margin: 6px;
  img {
    width: 60%;
    border-radius: 100%;
    margin: auto;
    display: block;
  }
  .wrap {
    box-shadow: 0 0 6px #cacaca;
    border-radius: 2px;
    font-size: 12px;
    padding: 6px;
    color: #818181;
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