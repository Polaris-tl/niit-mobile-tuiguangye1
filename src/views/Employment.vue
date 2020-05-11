<template>
  <div class="about">
    <Section title="最新就业情况">
      <ListScroll />
    </Section>

    <p class="ttt">高薪就业就在身边</p>
    <Gaoxin />
    <Button class="button"/>
    <img src="@/assets/employment/step.png" alt style="margin-bottom: 7px;"/>

    <p class="ttt">校企合作 双赢互惠</p>
    <S1 />
    <Button class="button"/>
    <p class="ttt">NIIT与多所大学签订合作协议</p>
    <S2 />
    <Button class="button"/>
  </div>
</template>

<script>
import Section from "@/components/Home/Section.vue";
import Button from "@/components/Common/Button.vue";

import Gaoxin from "@/components/Employment/Gaoxin.vue";
import ListScroll from "@/components/Employment/ListScroll.vue";
import S1 from "@/components/Employment/S1.vue";
import S2 from "@/components/Employment/S2.vue";

export default {
  components: {
    Section,
    Gaoxin,
    Button,
    ListScroll,
    S1,
    S2
  }
};
</script>


<style lang="less" scoped>
.button{
      margin: 17px auto 20px auto;
}
.ttt {
      font-size: 18px;
    color: #ce282e;
    font-weight: bold;
    line-height: 2.2;
    margin-bottom: 8px;
    text-align: center;
}
</style>