<template>
  <div class="foot">
    <div class="copyright">
      <p>©2019-2029重庆互联网NIIT学院版权所有 | 报名电话：023-63561996 | 地址：重庆市两江新区大竹林华山南路16号</p>
    </div>
    <div class="button">
      <div>
        <img src="@/assets/index/01.png" alt="">
        <p>了解专业</p>
      </div>
      <div>
        <img src="@/assets/index/02.png" alt="">
        <p>在线咨询</p>
      </div>
      <div>
        <img src="@/assets/index/03.png" alt="">
        <p>电话咨询</p>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
img {
}
.foot{
  .copyright{
    background: #707070;
    color: #fff;
    font-size: 11px;
    padding:2%;
  }
  .button{
    display: flex;
    justify-content: space-around;
    flex-grow:1;
    font-size: 14px;
    img{
      width: auto;
      height:16px
    }
    > div{
      display: flex;
      align-items: center;
      justify-content: center;
      padding:0 1%;
      height: 40px;
      line-height:40px;
      width: 100%;
      text-align: center;
      background: #2fa0ff;
      color: #fff;
      &:nth-child(2){
        background: #12d5ff;
      }
      p{
        margin-left: 3px;
      }
    }
  }
}
</style>