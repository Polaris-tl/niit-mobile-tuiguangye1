<template>
  <ul>
    <li>
      <div class="clearfix title">
        <div class="fl left">01</div>
        <div class="fl right">
          <p>国际学校</p>
          <p>International</p>
        </div>
        <p>全球排名第二，亚洲排名第一</p>
      </div>
      <div>
        <img src="@/assets/index/ys1.jpg" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">02</div>
        <div class="fl right">
          <p>师资雄厚</p>
          <p>Teachers</p>
        </div>
        <p>5-10年业内高水准老师团队</p>
      </div>
      <div>
        <img src="@/assets/index/ys2.jpg" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">03</div>
        <div class="fl right">
          <p>课程一线</p>
          <p>Courses</p>
        </div>
        <p>500人国际教师团队研发</p>
      </div>
      <div>
        <img src="@/assets/index/ys3.jpg" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">04</div>
        <div class="fl right">
          <p>环境一流</p>
          <p>Enviroment</p>
        </div>
        <p>2018年全新校区设备</p>
      </div>
      <div>
        <img src="@/assets/index/ys4.jpg" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">05</div>
        <div class="fl right">
          <p>就业保障</p>
          <p>Employment</p>
        </div>
        <p>毕业学生100%安置就业</p>
      </div>
      <div>
        <img src="@/assets/index/ys5.png" alt />
      </div>
    </li>
    <li>
      <div class="clearfix title">
        <div class="fl left">06</div>
        <div class="fl right">
          <p>免费试学</p>
          <p>Free trial</p>
        </div>
        <p>重庆市政府重点引进IT学校</p>
      </div>
      <div>
        <img src="@/assets/index/ys6.png" alt />
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
    &:not(:first-of-type) {
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
      .right {
        float: right;
        p {
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
      > p {
            clear: both;
    font-size: 12px;
    color: #636363;
    overflow: hidden;
    margin: 11px 5px 4px 5px;
      }
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
        font-size: 12px;
        color: #a6a6a6;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
      }
    }
  }
}
</style>>