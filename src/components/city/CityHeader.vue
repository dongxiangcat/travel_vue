<template>
  <div class="cityheader">
    <div class="header">
      <router-link to="/">
      <div class="back">
        <div class="iconfont back-icon">
          <svg class="icon svg-icon" aria-hidden="true">
            <use xlink:href="#icon-houtui"></use>
          </svg>
        </div>
      </div>
      </router-link>
      <div class="title">城市选择</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.header
  width:100%
  height: $headerHeight
  position relative
  background-color #00bcd4
  color white
  text-align center
  line-height $headerHeight
  font-size .32rem
  .back
    position absolute
    width: .4rem
    line-height .88rem
    padding-left .2rem
    padding-left .2rem
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

</style>
