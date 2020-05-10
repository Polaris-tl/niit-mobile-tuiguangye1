<template>
  <div>
    <swiper :options="swiperOptions">
      <swiper-slide v-for="item in devData" :key="item.year">
        <div class="box">
          <p class="year">{{item.year}}</p>
          <p class="detail">{{item.detail}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default {
  data() {
    return {
      swiperOptions: {
        spaceBetween: 44,
        slidesPerView: 2.5,
        freeMode:true
      },
      devData: [
        {
          year: 1997,
          detail: "1997年，NIIT进入中国"
        },
        {
          year: 1998,
          detail: "1997年，NIIT进入中国"
        },
        {
          year: 1999,
          detail: "1997年，NIIT进入中国"
        },
        {
          year: 2000,
          detail: "1997年，NIIT进入中国"
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
  &::after {
    content: "";
    width: 15px;
    height: 30px;
    position: absolute;
    top: 0;
    bottom: 0;
    margin: auto;
    right: -34px;
    background:url("~@/assets/about/rightArrow.png")  no-repeat;
        background-size: contain;
  }
  .year {
    margin-top: 30px;
    font-size: 22px;
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
    font-size: 14px;
    color: rgb(255, 255, 255);
    padding: 10px 6px 0 6px;
  }
}
</style>