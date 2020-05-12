<template>
  <div class="wrap">
    <p class="title">学员就业薪资表</p>
    <div class="bigbox">
      <div class="listTitle">
        <p class="name">姓名</p>
        <p class="major">专业</p>
        <p class="employment">就业</p>
        <p class="salary">薪资</p>
      </div>
      <div class="marquee-wrap">
        <ul :class="{'animate-up': animateUp}">
          <li v-for="(item, index) in listData" :key="index">
            <p class="name">{{item.name}}</p>
            <p class="major">{{item.major}}</p>
            <p class="employment">{{item.employment}}</p>
            <p class="salary">{{item.salary}}</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "ListScroll",
  data() {
    return {
      animateUp: false,
      listData: [
        {
          name: "白*",
          major: "嵌入式开发工程师",
          employment: "美**生物科技有限公司",
          salary: "11000元"
        },
        {
          name: "阔*里",
          major: "UI设计师",
          employment: "美**信息科技有限公司",
          salary: "9000元"
        },
        {
          name: "陈*力",
          major: "嵌入式开发工程师",
          employment: "软**力信息技术有限公司",
          salary: "9000元"
        },
        {
          name: "余*天",
          major: "VR建模设计师",
          employment: "创彩**广告制作有限公司",
          salary: "8000元"
        },
        {
          name: "杨*平",
          major: "Linux系统运维工程师",
          employment: "科**飞信息科技有限公司",
          salary: "7500元"
        },
        {
          name: "易*",
          major: "Web前端工程师",
          employment: "新*讯信息科技有限公司",
          salary: "8000元"
        },
        {
          name: "刘*生",
          major: "java软件开发工程师",
          employment: "重庆感*科技有限公司",
          salary: "12000元"
        },
        {
          name: "行*宗",
          major: "UI设计师",
          employment: "星**动广告传媒有限公司",
          salary: "7000元"
        },
        {
          name: "宫*旭",
          major: "Web前端工程师",
          employment: "小*科技有限公司",
          salary: "9000元"
        },
        {
          name: "童*飞",
          major: "java软件开发工程师",
          employment: "华*科技",
          salary: "9000元"
        },
        {
          name: "棋*美",
          major: "UI设计师",
          employment: "重庆装*设计有限公司",
          salary: "8500元"
        },
        {
          name: "鹏*天",
          major: "Web前端工程师",
          employment: "物**云信息科技有限公司",
          salary: "8000元"
        },
        {
          name: "林*",
          major: "java软件开发工程师",
          employment: "重庆影*科技有限公司",
          salary: "8000元"
        },
        {
          name: "张*贵",
          major: "UI设计师",
          employment: "成都生*科技有限公司",
          salary: "4000元"
        },
        {
          name: "乔*达",
          major: "java软件开发工程师",
          employment: "传**科技有限公司",
          salary: "11000元"
        }
      ],
      timer: null
    };
  },
  mounted() {
    this.timer = setInterval(this.scrollAnimate, 2500);
  },
  methods: {
    scrollAnimate() {
      this.animateUp = true;
      setTimeout(() => {
        this.listData.push(this.listData[0]);
        this.listData.shift();
        this.animateUp = false;
      }, 500);
    }
  },
  destroyed() {
    clearInterval(this.timer);
  }
};
</script>

<style lang="less" scoped>
.wrap {
  width: 94%;
  margin: 0 auto;
  border-radius: 4px;
  overflow: hidden;
  box-shadow: 0 0 6px #bfbfbf;
  background: #f5f8fa;
  .title {
    background: #ffba58;
    color: #eee;
    font-size: 16px;
    font-weight: bold;
    text-align: center;
    line-height: 30px;
    height: 30px;
  }
  .bigbox {
    background: #fff;
    box-shadow: 0 0 2px #c7c7c7;
    margin: 8px;
    border-radius: 4px;
    .marquee-wrap {
      height: 190px;
      overflow: hidden;
      ul {
        position: relative;
        li {
          height: 100%;
          text-overflow: ellipsis;
          overflow: hidden;
          white-space: nowrap;
          list-style: none;
          line-height: 36px;
          text-align: center;
          color: #4c4c4c;
          font-size: 14px;
          border-bottom: dashed 1px #d2d2d2;
          margin: 0 6px;
          font-weight: 400;
          p {
            float: left;
            font-size: 12px;
            text-align: center;
            white-space: nowrap;
            text-overflow: ellipsis;
          }
          .name {
            width: 15%;
            overflow: hidden;
          }
          .major {
            width: 35%;
            overflow: hidden;
          }
          .employment {
            width: 35%;
            overflow: hidden;
          }
          .salary {
            width: 15%;
            overflow: hidden;
          }
        }
      }
      .animate-up {
        transition: all 0.5s ease-in-out;
        transform: translateY(-36px);
      }
    }
  }
}
.listTitle {
  overflow: hidden;
  height: 41px;
  line-height: 41px;
  font-size: 14px;
  color: #3c3c3c;
  font-weight: bold;
  margin-bottom: 2px;
  margin: 0 6px;
  border-bottom: 1px solid #dedede;
  p {
    float: left;
    font-size: 12px;
    text-align: center;
    white-space: nowrap;
    text-overflow: ellipsis;
  }
  .name {
    width: 15%;
  }
  .major {
    width: 35%;
  }
  .employment {
    width: 35%;
  }
  .salary {
    width: 15%;
  }
}
</style>

