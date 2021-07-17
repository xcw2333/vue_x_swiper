<template>
  <div>
    <swiper>
      <swiper class="swiper" :options="swiperOption">
        <swiper-slide>Slide 1</swiper-slide>
        <swiper-slide>Slide 2</swiper-slide>
        <swiper-slide>Slide 3</swiper-slide>
        <swiper-slide>Slide 4</swiper-slide>
        <swiper-slide>Slide 5</swiper-slide>
        <swiper-slide>Slide 6</swiper-slide>
        <swiper-slide>Slide 7</swiper-slide>
        <swiper-slide>Slide 8</swiper-slide>
        <swiper-slide>Slide 9</swiper-slide>
        <swiper-slide>Slide 10</swiper-slide>
        <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div>
      </swiper>
    </swiper>
  </div>
</template>

<script>
  import Swiper from 'swiper'
  export default {
    name:'About',
    data(){
      return {
      }
    },
    mounted() {
      new Swiper ('.swiper-container', {
        loop: true,
        // 如果需要分页器
        pagination: '.swiper-pagination',
        // 如果需要前进后退按钮
        nextButton: '.swiper-button-next',
        prevButton: '.swiper-button-prev',
        // 如果需要滚动条
        // scrollbar: '.swiper-scrollbar',
        //如果需要自动切换海报
        // autoplay: {
        //   delay: 1000,//时间 毫秒
        //   disableOnInteraction: false,//用户操作之后是否停止自动轮播默认true
        // },
      })
    }
  }
</script>