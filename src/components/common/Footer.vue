<template>
<div class="footer">
  <div class="menu">
    <span class="item">机票</span>
    <span class="item">酒店</span>
    <span class="item">公寓</span>
    <i class="fenge">|</i>
    <span class="item">更多</span>
  </div>
  <div class="myinfo border-bottom">
    <span class="item">登录</span>
    <span class="item">我的订单</span>
    <span class="item">关于我们</span>
    <span class="item">最近浏览</span>
  </div>
  <div class="edition">
    <span class="item">触屏版</span>
    <span class="item activie">电脑版</span>
  </div>
  <div class="copyright">Qunar 京ICP备05021087</div>
</div>
</template>

<script>
export default {
  name: 'CommonFooter'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.footer
  height 2.72rem
  overflow hidden
  display flex
  flex-direction column
  .menu
    height .6rem
    line-height .6rem
    margin 0 auto
    font-size .24rem
    .item
      display block
      float left
      margin 0 .2rem
      color #9e9e9e
    .fenge
      display block
      float left
      color #9e9e9e
  .myinfo
    height .8rem
    line-height .8rem
    font-size .28rem
    .item
      display block
      margin-left .4rem
      float left
      color: $bgColor
  .border-bottom
    &:before
      border-color: #cacaca
      border-width .08rem
    &:after
      border-color: #cacaca
      border-width .08rem
  .edition
    height .6rem
    line-height .6rem
    margin 0 auto
    .item
      margin 0 .24rem
  .copyright
    flex 1
    display:flex
    align-items:center
    margin 0 auto
    color #9e9e9e
    vertical-align: middle;
</style>
