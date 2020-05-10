<template>
    <ul class="clearfix">
        <li>
          <img src="@/assets/index/k1.jpg" alt />
          <div>
            <p>云开发软件工程师</p>
          </div>
        </li>
        <li>
          <img src="@/assets/index/k2.jpg" alt />
          <div>
            <p>4D动漫游戏设计师</p>
          </div>
        </li>
        <li>
          <img src="@/assets/index/k3.jpg" alt />
          <div>
            <p>大数据运营工程师</p>
          </div>
        </li>
        <li>
          <img src="@/assets/index/k4.jpg" alt />
          <div>
            <p>UI设计师</p>
          </div>
        </li>
        <li>
          <img src="@/assets/index/k5.jpg" alt />
          <div>
            <p>电子竞技运动与管理</p>
          </div>
        </li>
        <li>
          <img src="@/assets/index/k6.jpg" alt />
          <div>
            <p>互联网+新零售</p>
          </div>
        </li>
      </ul>
</template>

<style lang="less" scoped>
  ul {
    li {
      float: left;
      width: 46%;
      margin: 0 2%;
      position: relative;
      margin-bottom: 11px;
      img {
        border-radius: 4px;
      }
      div {
        position: absolute;
        bottom: 4px;
        left: 0;
        right: 0;
        height: 30px;
        margin: auto;
        border-radius: 0 0 4px 4px;
        background-image: linear-gradient(
          0deg,
          rgba(0, 0, 0, 0.45882) 0%,
          rgba(0, 0, 0, 0.23) 63%,
          rgba(0, 0, 0, 0) 100%
        );
        p {
          font-size: 16px;
          font-weight: bold;
          color: #fff;
          text-align: center;
          position: relative;
          top: 5px;
        }
      }
    }
  }
</style>