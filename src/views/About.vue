<template>
  <div class="hhd">
    <Section title="校园环境" url="https://www.baidu.com" class="s1">
      <div class="box" ref="box">
        <img src="@/assets/about/50.jpg" alt />
        <p>NIIT隶属于重庆两江新区安道服务外包软件职业学校投资建设，重庆互联网学院是两江新区管委会在市委市政府的统一部署下，依托重庆互联网产业园的优势资源，为解决重庆互联网中高端人才缺口而建设的国内首个互联网学院，引进NIIT在通过互联网学院与互联网产业园相互融合、相互促进，推动重庆互联网人才队伍的建设和发展。学校总建筑面积约16万平方米，按照智慧校园、未来生活的理念 建设，能同时提供10000名学员的综合学习和2000名学员的住宿及生活配套服务。</p>
        <p>1997年，NIIT进入中国，凭借全球统一的教学模式，高质量的管理体系和与时俱进的课程内容，NIIT迅速成为中国IT职业教育领域的领先者。今天，NIIT已在中国25个省建立了超过183个授权培训中心，并与各大软件园、IT公司和大学建立了广泛的合作关系，每年都为中国培养大量的专业人才</p>
      </div>
      <More @click.native="handleMoreClick" ref="more" :isBoxCollapse="isBoxCollapse" />
    </Section>

    <Section title="发展历程" url="https://www.baidu.com">
      <swiper>
        <swiper-slide>1111</swiper-slide>
        <swiper-slide>2222</swiper-slide>
        <swiper-slide>1113331</swiper-slide>
      </swiper>
      <Button />
    </Section>

    <Section title="优秀师资力量" url="https://www.baidu.com">
      <Teachers />
      <Button />
    </Section>

    <Section title="环境设施" url="https://www.baidu.com" class="s4">
      <p>优质的校园环境能给学生更好的体验，为保障学生学习，在校区为学生提供优质的住宿环境、安全卫生的饮食，并开展多项互动互动让学生劳逸结合，学习质量更佳。</p>
      <Picture />
    </Section>
  </div>
</template>

<script>
import Section from "@/components/Home/Section.vue";
import Button from "@/components/Common/Button.vue";

import More from "@/components/About/More.vue";
import Teachers from "@/components/About/Teachers.vue";
import Picture from "@/components/About/Picture.vue";

export default {
  name: "About",
  data: () => {
    return {
      isBoxCollapse: true,
      initHeight: "193px"
    };
  },
  components: {
    Section,
    More,
    Button,
    Teachers,
    Picture
  },
  methods: {
    handleMoreClick: function() {
      console.log("asdasd");
      this.$refs.box.style.maxHeight =
        this.$refs.box.style.maxHeight == "1000px" ? "193px" : "1000px";
      this.isBoxCollapse = !this.isBoxCollapse;
    }
  }
};
</script>

<style lang="less" scoped>
.s1 {
  margin: 0 16px;
  position: relative;
  .box {
    max-height: 193px;
    transition: all 0.4s;
    overflow: hidden;
    img {
      float: left;
      width: 45%;
      margin-right: 28px;
      margin-bottom: 5px;
    }
    p {
      text-indent: 24px;
      color: #535353;
      font-size: 14px;
      line-height: 16px;
      line-height: 2;
    }
  }
}
.s4 {
  > p {
    font-size: 14px;
    color: #535353;
    text-align: justify;
    line-height: 1.8;
    text-indent: 39px;
    margin-top: 12px;
    width: 92%;
    margin: 12px auto 0 auto;
  }
}
</style>
