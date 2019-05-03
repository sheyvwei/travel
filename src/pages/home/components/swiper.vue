<template>
  <div class="wrapper">
    <!-- 使用轮播图使用这个模板 -->
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgURL"/>
      </swiper-slide>

      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
      <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
      <!-- <div class="swiper-scrollbar"   slot="scrollbar"></div> -->
    </swiper>
  </div>
</template>
<script>
export default{
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev'
        },
        pagination: '.swiper-pagination',
        loop: true // 可以循环
      },
      swiperList: [{
        id: '0001',
        imgURL: 'http://photo.tv.yundousoft.com/comic/focus/2017/01/09/20170109091700383.jpg/pic_380.jpg'
      }, {
        id: '0002',
        imgURL: 'http://photo.tv.yundousoft.com/comic/focus/2018/07/201807230018.jpg/pic_380.jpg'
      }, {
        id: '0003',
        imgURL: 'http://photo.tv.yundousoft.com/comic/focus/2016/12/29/20161229035524924.jpg/pic_380.jpg'
      }]

    }
  }
}
</script>
<style lang="stylus"  scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background : #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom : 63.15%
    background : #eee
    .swiper-img
      width: 100%
</style>
