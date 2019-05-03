<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom">
        <img class="item-img" src="http://img1.qunarzz.com/sight/p0/1504/e6/e64e8d217fe5a746.water.jpg_200x200_9d43b2ce.jpg"/>
        <div class="item-info">
          <p class="item-title">鼓浪屿海底世界</p>
          <p class="item-desc">浪漫厦门首站，浪漫的海洋公园</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default{
  name: 'HomeRecommend'
}
</script>
<style lang="stylus" scoped>
  .title
    margin-top : .2rem
    line-height : .8rem
    background: #eee
    text-indent : .2rem
  .item
    overflow: hidden
    display: flex
    height: 1.9rem
    // background: red
    .item-img
      width: .1.7rem
      height: .1.7rem
      padding: .1.7rem
    .item-info
      flex: 1
      padding: .1rem
      .item-title
        line-height: .54rem
        font-size: .32rem
      .item-desc
        line-height: .4rem
        color: #cccccc
      .item-button
        // line-height:
        margin-top: .2rem
        // background: red
        background: #ff9300
        padding: 0 .1rem
        border-radius: .06rem
        color: #fff
</style>
