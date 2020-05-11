<template>
  <swiper :options="swiperOptions">
    <swiper-slide v-for="(stu,index) in students" :key="index">
      <div class="hack">
        <div class="wrap">
          <img src="@/assets/index/xs1.png" alt />
          <div>
            <p class="p1">{{stu.name}}</p>
            <p class="p2">公司：{{stu.company}}</p>
            <p class="p3">
              月薪：
              <span>{{stu.salary}}</span>
            </p>
          </div>
        </div>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>

export default {
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 2.5
      },
      students:[
        {
          name:"彭磊",
          company:"视腾信息",
          salary:"7000"
        },
        {
          name:"彭磊",
          company:"视腾信息",
          salary:"7000"
        },
        {
          name:"彭磊",
          company:"视腾信息",
          salary:"7000"
        }
      ]
    };
  }
};
</script>

<style lang="less" scoped>
.hack {
  margin: 10px;
  .wrap {
    box-shadow: 0 0 6px rgba(212, 212, 212, 0.9490196078431372);
    background: #fff;
    padding: 5px;
    border-radius: 2px;
    font-size: 14px;
    .p1 {
      font-size: 16px;
      font-weight: bold;
    }
    span {
      color: #ff1f1f;
    }
  }
}
</style>