<template>
    <div class="city-list" ref="wrapper">
      <div>
      <div class="area-tab">
        <span class="active border">境内</span>
        <span class="border">境外 港澳台</span>
      </div>
      <h2 class="title">热门城市</h2>
      <ul class="list hot-city">
        <li v-for="item of hotCities" @click="handleClickCity(item.name)">{{item.name}}</li>
      </ul>
      <h2 class="title">字母排序</h2>
      <ul class="letter">
        <li v-for="(item,key) of cities" :key="key" @click="handleClickLetter">{{key}}</li>
      </ul>
      <div v-for="(citylist,key) of cities" :key="key" :ref="key">
        <h2 class="title">{{key}}</h2>
        <ul class="list item-city">
          <li v-for="item of citylist" @click="handleClickCity(item.name)">{{item.name}}</li>
        </ul>
      </div>
    </div>
    </div>
</template>

<script>
import Bscroll from 'better-scroll'
import { mapMutations } from 'vuex'
export default {
  name: 'CityList',
  mounted () {
    this.scroll = new Bscroll(this.$refs.wrapper)
  },
  props: {
    hotCities: Array,
    cities: Object
  },
  methods: {
    handleClickLetter (e) {
      const elem = this.$refs[e.target.innerHTML][0]
      this.scroll.scrollToElement(elem)
    },
    handleClickCity (city) {
      this.changeCity(city)
      this.$router.push('/')
    },
    ...mapMutations(['changeCity'])
  }
}
</script>

<style lang="stylus" scoped>
.city-list
  width 100%
  position absolute
  overflow hidden
  left 0
  top .88rem
  bottom 0
  background #f5f5f5
  .area-tab
    height .86rem
    line-height .86rem
    margin 0 auto
    display flex
    justify-content center
    align-items center
    background-color #00bcd4
    span
      display block
      width 42%
      text-align center
      height .4rem
      line-height .4rem
      font-size .28rem
      color white
    .active
      color #00bcd4
      background white
    .border
      &:before
        border-width .1rem
        border-color white
  .title
    height .24rem
    display block
    line-height .24rem
    font-size .24rem
    margin .24rem .3rem
  .list
    background white
    position relative
    overflow hidden
    z-index 0
    li
      float left
      width 33.33%
      height .9rem
      line-height .9rem
      font-size .28rem
      text-align center
      color: #212121
      border-bottom .02rem solid #ddd
      margin-bottom -2px
      z-index 10000
  .hot-city
    &:before
      content ''
      position absolute
      width 33.33%
      left 33.33%
      height 100%
      border-left .02rem solid #ddd
      border-right .02rem solid #ddd
      z-index -1
  .item-city
    &:before
      content ''
      position absolute
      width 25%
      left 25%
      height 100%
      border-left .02rem solid #ddd
      border-right .02rem solid #ddd
      z-index -1
    &:after
      content ''
      position absolute
      width 25%
      left 75%
      height 100%
      border-left .02rem solid #ddd
      z-index -1
    li
      width 25%
  .letter
    overflow hidden
    background white
    li
      float left
      width 16.66%
      height .9rem
      line-height .9rem
      font-size .28rem
      text-align center
      color: #212121
</style>
