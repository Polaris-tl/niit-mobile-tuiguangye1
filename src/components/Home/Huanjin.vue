<template>
  <div class="xyhj clearfix">
    <div class="left fl">
      <SmallHead title1="丰富的课余生活" title2="学生组织打篮球" />
      <img src="@/assets/index/xyhj-1.png" alt />
    </div>
    <div class="right fl">
      <SmallHead title1="便利的生活设施" title2="寝室安静舒适" />
      <swiper ref="mySwiper" :options="swiperOptions">
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
      </swiper>
      <SmallHead title1="完善的设施设备" title2="教室设备完美保障" />
      <swiper ref="mySwiper" :options="swiperOptions">
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/index/banner.jpg" alt style="width:100%" />
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
import SmallHead from "@/components/Home/SmallHead.vue";
export default {
  name: "Huanjin",
  components: {
    SmallHead
  },
  data() {
    return {
      swiperOptions: {
        spaceBetween: 10,
        slidesPerView: 2
      }
    };
  }
};
</script>

<style lang="less" scoped>
.xyhj {
  img {
    width: 80%;
    display: block;
    margin: auto;
    margin-top: 20px;
  }
  .left {
    width: 50%;
    box-sizing: border-box;
    border-right: 1px solid #eee;
    overflow: hidden;
    padding: 10px 10px;
  }
  .right {
    width: 50%;
    overflow: hidden;
    box-sizing: border-box;
    padding: 10px 10px;
    img {
      margin-top: 10px;
      margin-bottom: 10px;
    }
  }
}
</style>