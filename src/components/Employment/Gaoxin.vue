<template>
  <swiper :options="swiperOptions">
    <swiper-slide>
      <div class="hack">
        <div class="wrap">
          <img src="@/assets/employment/ttt.png" alt />
          <p class="name">谢昆</p>
          <p class="salary">
            月薪：
            <span>7000</span>
          </p>
          <p class="position">后端架构师</p>
          <p class="conpany">重庆哈哈哈及时有限公司</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="hack">
        <div class="wrap">
          <img src="@/assets/employment/ttt.png" alt />
          <p class="name">谢昆</p>
          <p class="salary">
            月薪：
            <span>7000</span>
          </p>
          <p class="position">后端架构师</p>
          <p class="conpany">重庆哈哈哈及时有限公司</p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="hack">
        <div class="wrap">
          <img src="@/assets/employment/ttt.png" alt />
          <p class="name">谢昆</p>
          <p class="salary">
            月薪：
            <span>7000</span>
          </p>
          <p class="position">后端架构师</p>
          <p class="conpany">重庆哈哈哈及时有限公司</p>
        </div>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>
export default {
  name: "Gaoxin",
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 2.5
      }
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