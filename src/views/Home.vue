<template>
  <div class="home">
    <div class="news">
      <p class="left">新闻<br />资讯</p>
      <div class="scroll">
        <span>热门</span><p>怎么打造自身职场技能？</p>
        <span>热门</span><p>怎么打造自身职场技能？</p>
      </div>
    </div>
    <img class="ydxx" src="@/assets/index/一地学习.png" alt="">
    <Section title="校园环境" url="https://www.baidu.com">ssssss</Section>
    <Section title="学校简介" url="https://www.baidu.com">ssssss</Section>
    <Section title="学校优势" url="https://www.baidu.com">ssssss</Section>
    <Section title="热门课程" url="https://www.baidu.com">ssssss</Section>
    <Section title="就业学员" url="https://www.baidu.com">ssssss</Section>
    <Section title="常见问题解答" url="https://www.baidu.com">ssssss</Section>
  </div>
</template>

<script>
import Section from '@/components/Home/Section.vue'

export default {
  name: 'Home',
  components: {
    Section
  }
}
</script>

<style lang="less" scoped>
  .news{
    overflow: hidden;
    border-top: 1px solid #eee;
    border-bottom: 1px solid #eee;
    padding: 10px 0;
    width: 96%;
    margin: 0 auto;
    color: #616161;
    letter-spacing: 2px;
    line-height: 20px;
    .left{
      font-size: 16px;
      font-weight: bold;
      margin-left: 10px;
      float: left;
      border-right: 1px solid #bdbdbd;
      padding-right: 17px;
    }
    .scroll{
      span{position: absolute;}
    }
  }
  .ydxx{
    width:100%
  }
</style>
