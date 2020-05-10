<template>
  <ul>
    <li>
      <div class="clearfix title">
        <div class="fl left">01</div>
        <div class="fl right">
          <p>教师团队</p>
          <p>Teacher Team</p>
        </div>
      </div>
      <div>
        <img src="@/assets/index/teacherteam.png" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">01</div>
        <div class="fl right">
          <p>教师团队</p>
          <p>Teacher Team</p>
        </div>
      </div>
      <div>
        <img src="@/assets/index/teacherteam.png" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">01</div>
        <div class="fl right">
          <p>教师团队</p>
          <p>Teacher Team</p>
        </div>
      </div>
      <div>
        <img src="@/assets/index/teacherteam.png" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">01</div>
        <div class="fl right">
          <p>教师团队</p>
          <p>Teacher Team</p>
        </div>
      </div>
      <div>
        <img src="@/assets/index/teacherteam.png" alt />
      </div>
    </li>
  </ul>
</template>


<style lang="less" scoped>
ul {
  background: url(~@/assets/index/ul-bg.png) repeat-y center;
  overflow: hidden;
  background-size: 3px;
  li {
    width: 45%;
    box-sizing: border-box;
    margin-left: 2%;
    position: relative;
    &:not(:first-of-type){
        margin-top: -10%;
    }
    &:nth-child(2n + 1) {
      margin-left: 53%;
    }
    &:nth-child(2n) {
      .left {
        float: right;
        &::before {
          content: "";
          width: 41%;
          height: 3px;
          background: #2fa0ff;
          position: absolute;
          top: 0;
          bottom: 0;
          margin: auto;
          right: -247%;
        }
      }
      .right{
          float: right;
          p{
              text-align: right;
          }
      }
    }
    img {
      width: 60%;
      margin: auto;
      display: block;
      margin-top: 16px;
    }
    .title {
      background: #fff;
      border-radius: 2px;
      padding: 2%;
      box-shadow: 0 0 8px #00000038;
    }
    .left {
      float: left;
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
      position: relative;
      &::before {
        content: "";
        width: 41%;
        height: 3px;
        background: #2fa0ff;
        position: absolute;
        top: 0;
        bottom: 0;
        margin: auto;
        left: -61%;
      }
    }
    .right {
      float: left;
      p:nth-child(1) {
        font-size: 16px;
        font-weight: bold;
        padding: 0 0 0px 4px;
        border-bottom: 2px solid #2fa0ff;
      }
      p:nth-child(2) {
        font-size: 14px;
        color: #a6a6a6;
      }
    }
  }
}
</style>>