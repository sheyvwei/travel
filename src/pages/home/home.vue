<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <div>防止窗口抖动  1.    overflow: hidden width: 100% height: 0 padding-bottom : 63.15%</div>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
export default {
  name: 'home',
  components: {
    HomeHeader,
    HomeSwiper
  }
}
</script>

<style>
</style>
