<template>
  <div class="home">

    <div class="news">
      <p class="left">
        新闻
        <br />资讯
      </p>
      <div class="scroll">
        <span>热门</span>
        <p>怎么打造自身职场技能？</p>
        <span>热门</span>
        <p>怎么打造自身职场技能？</p>
      </div>
    </div>

    <img class="ydxx" src="@/assets/index/一地学习.png" alt />
    <Section title="校园环境" url="https://www.baidu.com" >
      <Huanjin />
    </Section>

    <Section title="学校简介" class="xxjj" url="https://www.baidu.com">
      <img src="@/assets/index/xxjj.png" alt />
      <p>重庆互联网学校总建筑面积约16万平方米，按照智慧校园、未来生活的理念建设，能同时提供10000名学员的综合学习和2000名学员的住宿及生活配套服务。NIIT建校39年,在重庆、上海、苏州、常州、海南、贵阳等多省市拥有多个IT直属分校，是我国权威的高端IT学院之一。致力于高端IT技术人才培养、输送，一直以“就业质量”为本，不仅看重学员的就业率，更注重学员的就业质量，以培养“实用型、创新型”人才为目标。</p>
    </Section>

    <Section title="学校优势" url="https://www.baidu.com">
      <Advantage />
    </Section>

    <Section title="热门课程" url="https://www.baidu.com">
      <HotClass />
    </Section>

    <Section title="就业学员" url="https://www.baidu.com">
      <Employment />
    </Section>

    <Section title="常见问题解答" url="https://www.baidu.com">
      <Question />
    </Section>
  </div>
</template>

<script>
import Section from "@/components/Home/Section.vue";
import Huanjin from "@/components/Home/Huanjin.vue";
import HotClass from "@/components/Home/HotClass.vue";
import Advantage from "@/components/Home/Advantage.vue";
import Employment from "@/components/Home/Employment.vue";
import Question from "@/components/Home/Question.vue";

export default {
  name: "Home",
  components: {
    Section,
    Huanjin,
    HotClass,
    Advantage,
    Employment,
    Question,
    
  }
  
};
</script>

<style lang="less" scoped>
.news {
  overflow: hidden;
  border-top: 1px solid #eee;
  border-bottom: 1px solid #eee;
  padding: 10px 0;
  width: 96%;
  margin: 0 auto;
  color: #616161;
  letter-spacing: 2px;
  line-height: 20px;
  .left {
    font-size: 16px;
    font-weight: bold;
    margin-left: 10px;
    float: left;
    border-right: 1px solid #bdbdbd;
    padding-right: 17px;
  }
  .scroll {
    span {
      position: absolute;
    }
  }
}
.xxjj {
  img {
    margin: auto;
    display: block;
    width: 66%;
    margin-top: 20px;
    margin-bottom: 16px;
  }
  p {
    width: 94%;
    margin: 0 auto;
    font-size: 14px;
    color: #535353;
    line-height: 1.7;
    text-indent: 24px;
    text-align: justify;
  }
}
.ydxx {
  width: 100%;
}
</style>
