<template>
  <div class="weekend">
    <div class="title">
      周末去哪儿
    </div>
    <div class="content">
      <ul>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">京城周末撒欢</div>
            <div class="item-desc">在帝都过周末，不仅仅是城中游！</div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">京城周末撒欢</div>
            <div class="item-desc">在帝都过周末，不仅仅是城中游！</div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">京城周末撒欢</div>
            <div class="item-desc">在帝都过周末，不仅仅是城中游！</div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/source/1811/f3/86173f863bef61.jpg_r_640x214_52b003ac.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">京城周末撒欢</div>
            <div class="item-desc">在帝都过周末，不仅仅是城中游！</div>
          </div>
        </li>

      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend'
}
</script>

<style lang="stylus" scoped>
  .weekend
    width: 100%
    display flex
    flex-direction: column
    .title
      height .8rem
      line-height .8rem
      font-size .28rem
      padding-left .26rem
      color #212121
    .content
      .content-item
        margin-bottom  .1rem
        .item-img
          width 100%
          height 0
          padding-bottom 36%
          img
            width 100%
        .item-content
          background-color white
          padding .14rem .24rem .24rem
          .item-name
            line-height .48rem
            font-size .28rem
            color #212121
          .item-desc
            font-size .24rem
            line-height .42rem
            color #616161
</style>
