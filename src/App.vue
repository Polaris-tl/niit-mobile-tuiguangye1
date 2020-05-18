<template>
  <div id="app">
    <!-- 头部 -->
    <Head />
    <Nav />
    <!-- banner -->
    <Banner />
    <!-- 导航 -->
    
    <!-- 路由容器 -->
    <router-view/>
    <!-- 尾部   -->
    <Foot />
  </div>
</template>


<script>
import Head from '@/components/Head.vue'
import Banner from '@/components/Banner.vue'
// import Nav from '@/components/Nav.vue'
import Nav from '@/components/New/Nav.vue'
import Foot from '@/components/Foot.vue'

export default {
  name: 'Home',
  components: {
    Head,
    Nav,
    Banner,
    Foot
  }
}
</script>>

<style lang="less">
*{margin: 0;padding:0;}
.fl{float: left;}
.fr{float: right;}
.clearfix::after{
  content: "";
  display: block;
  height: 0;
  clear: both;
}
li{list-style: none;}
a{text-decoration: none;}
</style>
