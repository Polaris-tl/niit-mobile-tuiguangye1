<template>
  <div class="head">
    <div class="fir">
      <img src="@/assets/index/logo-blue.png" alt="logo" />
    </div>
    <div class="sec">
      <p>重庆互联网学院</p>
      <p>CHONG QING INTERNET INSITUTE</p>
    </div>
    <!-- <div class="thi">
      <p>咨询热线</p>
      <p>023-6356 1996</p>
    </div> -->
  </div>
</template>

<style lang="less" scoped>
.head {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 2% 1%;
  overflow: hidden;
  > div {
    padding: 0 1%;
  }
  .fir {
    width:20%;
    img {
      width: 100%;
    }
  }
  .sec{
    p:nth-child(1){
      font-size: 16px;
      font-family: "Microsoft YaHei";
      color: rgb(97, 97, 97);
      font-weight: bold;
      line-height: 1.2;
    }
    p:nth-child(2) {
      font-size: 10px;
      font-family: "Microsoft YaHei";
      color: rgb(97, 97, 97);
      line-height: 1.2;
    }
  }
  .thi{
    p{
      font-size: 15px;
      font-family: "Microsoft YaHei";
      color: rgb(97, 97, 97);
      font-weight: bold;
      line-height: 1.35;
    }
  }
}
</style>