<script setup>
import {Vue3SeamlessScroll} from "vue3-seamless-scroll";
import {reactive, ref} from "vue";

const list = reactive([
  '../../assets/images/partner/binance.webp',
  '../../assets/images/partner/bloomberg.webp',
  '../../assets/images/partner/bridgewater.webp',
  '../../assets/images/partner/coindesk.webp',
  '../../assets/images/partner/ecb.webp',
  '../../assets/images/partner/fireblocks.webp',
  '../../assets/images/partner/forbes.webp',
  '../../assets/images/partner/ft.webp',
  '../../assets/images/partner/vaneck.webp',
  '../../assets/images/partner/wsj.webp'
])

const classOptions = {
  step: 5
};

</script>

<template>
  <div class="demo">
    <vue3-seamless-scroll :list="list" :step="0.3" :hover="true" :singleLine="true" :direction="'left'" class="scroll-wrap ulwarp li2 ul">




      <ul class="ui-wrap">
<!--        <li class="li-item" v-for="(item,i) of list" :key="i">-->
<!--          <img :src="item" alt="">-->
<!--        </li>-->

        <li class="li-item"><img src="@/assets/images/partner/binance.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/bridgewater.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/coindesk.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/ecb.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/fireblocks.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/forbes.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/ft.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/vaneck.webp" alt=""> </li>
        <li class="li-item"><img src="@/assets/images/partner/wsj.webp" alt=""> </li>
      </ul>

    </vue3-seamless-scroll>
  </div>
</template>

<style lang="less" scoped>
.demo {
  //display: flex;
  //align-items: center;
  //justify-content: center;

  //max-width: 1280px;

  margin-top: 40px;

}
.scroll-wrap {
  //height:64px;
  //width: 1280px;
  overflow: hidden;
}

@media (min-width: 1280px) {
  .scroll-wrap {
    max-width: 1280px;
  }
}

.ui-wrap {
  display: flex;
  list-style: none;

  margin:0;
  padding:0;

  max-width: 1280px;
}
.li-item {
  padding:0;
  margin-top:0;
  //margin-left: 20px;
  width: 600px;
  //height: 128px;
  //line-height: 200px;
  //text-align: center;
  //font-size: 28px;
  //background-color: rgb(171, 167, 168);

}
</style>
