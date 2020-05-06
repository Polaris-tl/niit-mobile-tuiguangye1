<template>
  <div id="app">
    <!-- 头部 -->
    <Head />
    <!-- banner -->
    <Banner />
    <!-- 路由 -->
    <Nav />
    <!-- 路由容器 -->
    <router-view/>
    <!-- 尾部   -->
    <Foot />
  </div>
</template>


<script>
import Head from '@/components/Head.vue'
import Banner from '@/components/Banner.vue'
import Nav from '@/components/Nav.vue'
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
a{text-decoration: none;}
</style>
