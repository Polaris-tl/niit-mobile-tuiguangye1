<template>
  <div>
    <swiper ref="mySwiper" :options="swiperOptions">
      <swiper-slide><img src="@/assets/index/banner.jpg" alt="" /></swiper-slide>
      <swiper-slide><img src="@/assets/index/banner2.jpg" alt="" /></swiper-slide>
      <swiper-slide><img src="@/assets/index/banner3.jpg" alt="" /></swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'Banner',
    data() {
      return {
        swiperOptions: {
          pagination: {
            el: '.swiper-pagination'
          },
          // Some Swiper option/callback...
        }
      }
    },
  computed: {
      swiper() {
        return this.$refs.mySwiper.$swiper
      }
    }
};
</script>

<style lang="less" >
.swiper-pagination-bullet-active{
  background: #fff;
  opacity: 0.8;
}
img{
  width:100%
}
</style>