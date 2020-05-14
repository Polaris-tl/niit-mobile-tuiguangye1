<template>
  <div class="news">
      <p class="left">
        新闻
        <br />资讯
      </p>
      <NewsScroll />
    </div>
</template>
<script>
import NewsScroll from "@/components/Home/NewsScroll.vue";
export default {
  name:"News",
  components:{
    NewsScroll
  }
}
</script>>


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
}
</style>>