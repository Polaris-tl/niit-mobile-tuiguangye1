<template>
  <div class="nav">
    <ul>
      <li>
        <router-link to="/">首页</router-link>
      </li>
      <li>
        <router-link to="/about">学校介绍</router-link>
      </li>
      <li>
        <router-link to="/enviroment">学校环境</router-link>
      </li>
      <li>
        <router-link to="/employment">就业信息</router-link>
      </li>
    </ul>
  </div>
</template>

<style lang="less" scoped>
.nav {
  ul {
    height: 34px;
    width: 98%;
    margin: 0 auto;
    font-family: "Microsoft YaHei";
    display: flex;
    align-items: center;
    justify-content: center;
    color: #333;
    font-size: 14px;
    font-weight: bold;
    li {
      padding-right: 14px;
      padding-left: 14px;
      line-height: 14px;
      border-right: 1px solid #000;
      &:first-child {
        padding-left: 0;
      }
      &:last-child {
        padding-right: 0;
        border: 0;
      }
      a {
        color: #333;
        &.router-link-exact-active {
          color: #0e80fc;
          font-weight: bold;
        }
      }
      
    }
  }
}
</style>