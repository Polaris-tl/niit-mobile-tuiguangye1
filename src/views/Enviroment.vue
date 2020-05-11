<template>
  <div class="about">
    <Section title="校园环境">
      <div class="description">安静/生机勃发/怡人/清香四溢</div>
      <div class="picBox clearfix">
        <div class="fl left">
          <img src="@/assets/enviroment/xxhj/26.jpg" alt />
          <img src="@/assets/enviroment/xxhj/27.jpg" alt />
          <img src="@/assets/enviroment/xxhj/42.jpg" alt />
          <img src="@/assets/enviroment/xxhj/43.jpg" alt />
        </div>
        <div class="fl left">
          <img src="@/assets/enviroment/xxhj/47.jpg" alt />
          <img src="@/assets/enviroment/xxhj/49.jpg" alt />
          <img src="@/assets/enviroment/xxhj/48.jpg" alt />
          <img src="@/assets/enviroment/xxhj/timg (1).jpg" alt />
        </div>
      </div>
    </Section>
    <Section title="上课环境">
      <div class="description">勤思/认真高效/实时解答/项目实战</div>
      <div class="picBox clearfix">
        <div class="fl left">
          <img src="@/assets/enviroment/skhj/75.jpg" alt />
          <img src="@/assets/enviroment/skhj/22.jpg" alt />
          <img src="@/assets/enviroment/skhj/25.jpg" alt />
        </div>
        <div class="fl left">
          <img src="@/assets/enviroment/skhj/24.jpg" alt />
          <img src="@/assets/enviroment/skhj/77.jpg" alt />
          <img src="@/assets/enviroment/skhj/23.jpg" alt />
        </div>
      </div>
    </Section>
    <Section title="寝室环境">
      <div class="description">书桌/衣柜/空调/wifi/电视</div>
      <div class="picBox clearfix">
        <div class="fl left">
          <img src="@/assets/enviroment/qs/11.jpg" alt />
          <img src="@/assets/enviroment/qs/IMG_5646.jpg" alt />
          <img src="@/assets/enviroment/qs/IMG_5634.jpg" alt />
          <img src="@/assets/enviroment/qs/7.jpg" alt />
        </div>
        <div class="fl left">
          <img src="@/assets/enviroment/qs/6.jpg" alt />
          <img src="@/assets/enviroment/qs/5.jpg" alt />
          <img src="@/assets/enviroment/qs/4.jpg" alt />
          <img src="@/assets/enviroment/qs/9.jpg" alt />
        </div>
      </div>
    </Section>
  </div>
</template>


<script>
import Section from "@/components/Home/Section.vue";
export default {
  name: "Enviroment",
  components: {
    Section
  }
};
</script>


<style lang="less" scoped>
.description {
  width: 80%;
    height: 25px;
    line-height: 23px;
    margin: 0 auto;
    text-align: center;
    color: #555555;
    font-size: 13px;
    margin-bottom: 4px;
    position: relative;
  &::before {
    content: "";
    width: 120px;
    height: 1px;
    display: block;
    position: absolute;
    left: 0;
    right: 0;
    margin: auto;
    top: 0;
    background: url("~@/assets/enviroment/common/titile-line.png");
    background-size: cover;
  }
  &::after {
    content: "";
    width: 120px;
    height: 1px;
    display: block;
    position: absolute;
    left: 0;
    right: 0;
    margin: auto;
    bottom: 0;
    background: url("~@/assets/enviroment/common/titile-line.png");
    background-size: cover;
  }
}
.picBox {
  background: #f7f7f7;
  padding: 0.5rem 0.1rem;
  position: relative;
  .left {
    width: 48%;
    margin: 0 1%;
    img {
      width: 94%;
      height: auto;
      margin: 5% 3%;
      border: 4px solid #fff;
      border-radius: 2px;
      box-shadow: 0 0 6px #a5a5a5;
    }
  }
  .bot {
    position: absolute;
    bottom: 0rem;
    left: 0;
  }
}
</style>