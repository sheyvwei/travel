<template>
    <div class="header">
        <div class="header-left">
           <div class="iconfont back-icon">&#xe624;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>输入内容
        </div>
        <div class="header-right">
            城市<span class="iconfont right-icon">&#xe738;</span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
    @import '~styles/varibles.styl'
    .header
        display: flex
        line-height: .86rem
        background: $bgColor
        color: #fff
        .header-left
            float: left
            width: .64rem
            .back-icon
                text-align: center
                font-size: .4rem
        .header-input
            line-height .64rem
            flex: 1
            height: .64rem
            padding-left: .2rem
            margin-left: .2rem
            margin-top: .12rem
            color: #ccc
            background: #fff
            border-radius .1rem
        .header-right
            width : 1.24rem
            float: right
            text-align: center
            .right-icon
                font-size : .24rem
</style>
