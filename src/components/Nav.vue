<template>
  <div class="nav">
    <ul>
      <li>
        <img src="@/assets/index/icon-1.png" alt="">
        <router-link to="/">首页</router-link> 
      </li>
      <li>
        <img src="@/assets/index/icon-2.png" alt="">
        <router-link to="/about">介绍</router-link>
      </li>
      <li>
        <img src="@/assets/index/icon-3.png" alt="">
        <router-link to="/enviroment">环境</router-link>
      </li>
      <li>
        <img src="@/assets/index/icon-4.png" alt="">
        <router-link to="/employment">就业</router-link>
      </li>
    </ul>
  </div>
</template>

<style lang="less" scoped>
.nav {
  padding: 15px 10px;
  font-size: 14px;
  ul{
    display: flex;
    li{
      list-style: none;
      text-align: center;
      img{
        width:75%;
        margin: 0 auto;
      }
      a {
      text-decoration: none;
      display: inline-block;
      color: #2c3e50;

      &.router-link-exact-active {
        color: #0e80fc;
        font-weight: bold;
      }
    }
  }
  }
}
</style>