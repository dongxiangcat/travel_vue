<template>
  <div class="header">
    <div class="back">
      <div class="iconfont back-icon">
        <svg class="icon svg-icon" aria-hidden="true">
          <use xlink:href="#icon-houtui"></use>
        </svg>
      </div>
    </div>
    <div class="search">
      <svg class="icon svg-icon search-icon" aria-hidden="true">
        <use xlink:href="#icon-sousuo"></use>
      </svg>
      <span class="search-desc">输入城市/景点/游玩主题</span>
    </div>
    <router-link to="/city">
    <div class="city">
      <div class="city-content">
        <span class="city-content-text">{{city}}</span>
        <svg class="icon svg-icon city-content-icon" aria-hidden="true">
          <use xlink:href="#icon-xiala"></use>
        </svg>
      </div>
    </div>
    </router-link>
  </div>
</template>

<script>
import '@/assets/styles/iconfont/iconfont.js'
import { mapState } from 'vuex'
export default {
  name: 'HomeHeader',
  computed: {
    ...mapState(['city'])
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.header
  width:100%
  height: $headerHeight
  display: flex
  background-color $bgColor
  .back
    width: .4rem
    line-height .88rem
    margin-left .2rem
    margin-right .2rem
    .back-icon
      font-size: .6rem
      text-align center
      fill: white
      .icon
        width: .8em
        height: 1em
        vertical-align: -0.15em
        fill: currentColor
        overflow: hidden
  .search
    flex: 1
    margin:.14rem 0
    height .6rem
    line-height .6rem
    border-radius .1rem
    background-color white
    display flex
    .search-icon
      width .36rem
      height .6rem
      margin-left .2rem
      margin-right .2rem
    .search-desc
      flex 1
      height .6rem
      line-height .6rem
      color: #e4e7ea
  .city
    width 1.32rem
    height:.88rem
    .city-content
      line-height .48rem
      height .48rem
      margin: .2rem auto
      width: .98rem
      color white
      .city-content-text
        height .48rem
        line-height .48rem
        display block
        float left
        margin-right .1rem
      .city-content-icon
        width .2rem
        height .2rem

</style>
