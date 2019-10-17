<template>
  <div class="main">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-icon></home-icon>
    <home-hot></home-hot>
    <home-guess></home-guess>
    <home-weekend></home-weekend>
    <common-footer></common-footer>
  </div>
</template>
<script>
// @ is an alias to /src
import HomeHeader from '@/components/home/HomeHeader'
import HomeSwiper from '@/components/home/HomeSwiper'
import HomeIcon from '@/components/home/HomeIcon'
import HomeHot from '@/components/home/HomeHot'
import HomeGuess from '@/components/home/HomeGuess'
import HomeWeekend from '@/components/home/HomeWeekend'
import CommonFooter from '@/components/common/Footer'
import { mapState } from 'vuex'

export default {
  name: 'home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeIcon,
    HomeHot,
    HomeGuess,
    HomeWeekend,
    CommonFooter
  },
  data () {
    return {
      lastCity: ''
    }
  },
  computed: {
    ...mapState(['city'])
  },
  mounted () {
    this.lastCity = this.city
  },
  activated () {
    if (this.lastCity !== this.city) {
      this.lastCity = this.city
      console.log('重新加载')
    }
  }
}
</script>
<style lang="stylus" scoped>
.main
  overflow scroll
  background-color #f5f5f5
</style>
