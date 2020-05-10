<template>
  <ul>
    <li class="clearfix">
      <div class="fl left">01</div>
      <div class="fl right">
        <p>教师团队</p>
        <p>Teacher Team</p>
      </div>
      <img src="@/assets/index/teacherteam.png" alt />
    </li>
  </ul>
</template>


<style lang="less" scoped>
ul {
  background: url(~@/assets/index/ul-bg.png) repeat-y center;
  li {
    width: 50%;
    box-sizing: border-box;
    .left {
      background: url(~@/assets/index/polygon.png) no-repeat;
      background-size: contain;
      background-position: center center;
      width: 40px;
      height: 40px;
      line-height: 40px;
      font-weight: bold;
      font-size: 16px;
      color: #fff;
      text-align: center;
    }
  }
}
</style>>