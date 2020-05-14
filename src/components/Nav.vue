<template>
  <div class="nav">
    <ul>
      <li>
        <router-link to="/">
          <img src="@/assets/index/icon-1.png" alt />
          <p>首页</p>
          
        </router-link>
      </li>
      <li>
        <router-link to="/about">
          <img src="@/assets/index/icon-2.png" alt />
          <p>介绍</p>
          
        </router-link>
      </li>
      <li>
        <router-link to="/enviroment">
          <img src="@/assets/index/icon-3.png" alt />
          <p>环境</p>
          
        </router-link>
      </li>
      <li>
        <router-link to="/employment">
          <img src="@/assets/index/icon-4.png" alt />
          <p>就业</p>
          
        </router-link>
      </li>
    </ul>
  </div>
</template>

<style lang="less" scoped>
.nav {
  padding: 15px 10px;
  font-size: 14px;
  ul {
    display: flex;
    li {
      list-style: none;
      text-align: center;
      img {
        width: 75%;
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