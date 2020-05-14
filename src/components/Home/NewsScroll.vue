<template>
  <div class="marquee-wrap">
    <ul :class="{'animate-up': animateUp}">
      <li v-for="(item, index) in listData" :key="index">
        <p>
          <span>{{item.tag}}</span>
          <a :href="item.url">{{item.title}}</a>
          
        </p>
      </li>
    </ul>
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
          tag: "热门",
          title: "怎么打造自身职场技能？",
          url:"http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn"
        },
        {
          tag: "热门",
          title: "如何把有限的精力用在刀刃上？",
          url:"http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn"
        },
        {
          tag: "热门",
          title: "零基础可以学IT技术吗？",
          url:"http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn"
        },
        {
          tag: "热门",
          title: "怎样才能做到学历工作双丰收？",
          url:"http://awt.zoosnet.net/LR/Chatpre.aspx?id=AWT24214282&lng=cn"
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
.marquee-wrap {
  height: 42px;
  overflow: hidden;
  ul {
    position: relative;
    li {
      height: 100%;
      text-overflow: ellipsis;
      overflow: hidden;
      white-space: nowrap;
      list-style: none;
      line-height: 21px;
      color: #4c4c4c;
      font-size: 12px;
      border-bottom: dashed 1px #d2d2d2;
      margin: 0 6px;
      font-weight: 400;
      span {
        position: absolute;
        left: 0px;
        background: #f00;
        color: #fff;
        display: block;
        width: 33px;
        text-align: center;
        height: 17px;
        border-radius: 4px;
        line-height: 17px;
        padding: 0px 3px;
        top: 0;
        bottom: 0;
        margin: auto;
        text-indent: 0px;
      }
      p {
        margin-left: 8px;
        position: relative;
        text-indent: 48px;
      }
      a{
        color: #4c4c4c;
      }
    }
  }
  .animate-up {
    transition: all 0.5s ease-in-out;
    transform: translateY(-21px);
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

