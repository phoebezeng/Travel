<template>
    <div class="header">
        <div class="header-left">
            <span class="iconfont back-icont">&#xe624;</span>
        </div>
        <div class="header-input"><span class="iconfont">&#xe613;</span>输入城市/景点/游玩主题</div>
        <div class="header-right">城市<span class="iconfont arrow-icont">&#xe6aa;</span></div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
.header
    line-height: .86rem
    background: #00bcd4
    color: #fff
    display: flex
    .header-left
        width: .64rem
        float: left
        .back-icont
            text-align: center
            font-size: .38rem
    .header-input
        flex: 1
        position: relative
        height: .64rem
        margin-top: .12rem
        background-color: #ffffff
        color: #ccc
        line-height: .64rem
        padding-left: .04rem
    .header-right
        width: 1.04rem
        padding: 0 .1rem
        float: right
        text-align: center
        .arrow-icont
            font-size: .34rem
            margin-left: .03rem
</style>
