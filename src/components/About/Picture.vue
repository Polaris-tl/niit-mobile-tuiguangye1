<template>
  <div class="content">
    <div class="opt clearfix" @click="handleClick">
      <span :class="{active:showId == 1}" :id="1">校园</span>
      <span :class="{active:showId == 2}" :id="2">宿舍</span>
      <span :class="{active:showId == 3}" :id="3">课堂</span>
    </div>
    <div class="pic clearfix" id="pic">
      <div class="xuexiao" v-show="showId == 1">
        <img src="@/assets/about/xy1.jpg" alt />
        <img src="@/assets/about/xy2.jpg" alt />
        <img src="@/assets/about/xy3.jpg" alt />
        <img src="@/assets/about/xy4.jpg" alt />
      </div>
      <div class="xuexiao" v-show="showId == 2">
        <img src="@/assets/about/qs1.jpg" alt />
        <img src="@/assets/about/qs2.jpg" alt />
        <img src="@/assets/about/qs3.jpg" alt />
        <img src="@/assets/about/qs4.jpg" alt />
      </div>
      <div class="xuexiao" v-show="showId == 3">
        <img src="@/assets/about/sk1.jpg" alt />
        <img src="@/assets/about/sk2.jpg" alt />
        <img src="@/assets/about/sk3.jpg" alt />
        <img src="@/assets/about/sk4.jpg" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      showId:1,
      intervalId:null
    }
  },
  methods:{
    handleClick: function(e){
      this.showId = e.target.id
    },
    autoplay: function(){
      this.showId++
      if(this.showId > 3){
        this.showId = 1
      }
    }
  },
  mounted(){
    this.intervalId = setInterval(this.autoplay,3500)
  },
  beforeDestroy(){
    clearInterval(this.intervalId)
  }
};
</script>

<style lang="less" scoped>
.clearfix:after {
  content: "";
  display: block;
  clear: both;
}
.content {
  width: 96%;
  margin: auto;
  padding: 13px 0 0 0;
  .opt {
    display: flex;
    justify-content: center;
    text-align: center;
    margin-bottom: 12px;
    span {
      margin: 0 2px;
      width: 24%;
      padding: 1% 0;
      font-size: 14px;
      border-radius: 2px;
      color: #fff;
      background: #bfbfbf;
      display: inline-block;
      position: relative;
    }
    .active {
      background-color: #23c7ff;
      color: #fff;
      &::after {
        content: "";
        position: absolute;
        width: 0;
        right: 0;
        margin: auto;
        left: 0;
        bottom: -16px;
        height: 0;
        border-width: 6px;
        border-style: solid;
        border-color: #23c7ff transparent transparent transparent;
      }
    }
  }
  .pic {
    img {
      float: left;
      width: 48%;
      margin: 1%;
    }
  }
}
</style>