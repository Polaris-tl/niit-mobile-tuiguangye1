<template>
  <div>
    <!-- <div class="title">
      <img src="@/assets/index/huanjin/title_decoration.png" alt />
      <p>学校环境</p>
      <p>Environment</p>
    </div> -->
    <div class="content">
      <p>优质的校园环境能给学生更好的体验，学习质量更佳。</p>
    </div>
    <div class="kkk">
      <swiper ref="mySwiper" :options="swiperOptions">
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/1.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/2.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/3.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/4.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/5.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/6.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/7.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/8.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/huanjin/new/9.jpg" alt style="width:100%" />
        </swiper-slide>
    </swiper>
    </div>
    
  </div>
</template>


<script>
export default {
  name: "Huanjin",
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 3,
        initialSlide :1,
        autoplay: {delay:3000},
      }
    };
  }
};
</script>

<style lang="less" scoped>
.swiper-slide{
  transition: 300ms;
}
.swiper-slide:not(.swiper-slide-next) {
    transform: scale(0.8);
}
.title {
  display: flex;
  width: 90%;
  margin: 0 auto;
  justify-content: flex-start;
  align-items: center;
  margin-top: 6px;
  margin-bottom: 8px;
  img {
    height: 15px;
    width: auto;
    padding-right: 3px;
  }
  p:first-of-type {
    font-size: 20px;
        color: #535353;
    font-weight: bold;
    margin-right: 4px;
    color: #404040;
    padding-bottom: 2px;
    border-bottom: 1px solid #7d7d7d;
  }
  p:last-of-type {
    font-size: 14px;
    font-weight: bold;
    color: #b9b9b9;
  }
}
.content {
  width: 96%;
  margin: 0 auto;
  p{
    padding: 0 10px;
    font-size: 14px;
    text-indent: 28px;
    line-height: 25px;
    letter-spacing: 1px;
    text-align: justify;
  }
}
</style>>