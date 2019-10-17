<template>
  <div class="home-swiper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide>
        <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1709/39/b98fdb3ee7478e02.jpg_750x200_be64b756.jpg">
      </swiper-slide>
      <swiper-slide>
        <img class="swiper-img" src="http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/201910/78b240572657a6da67e662540c846dd6.jpg_750x200_b75c8be9.jpg">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
import  { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'HomeSwiper',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      swiperOption: {
        loop: true,
        spaceBetween: 5,
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        }

      }
    }
  }
}
</script>
<style lang="stylus" scoped>
.home-swiper >>> .swiper-pagination-bullet-active
  background-color white !important
.home-swiper
  width 100%
  overflow hidden
  height 0
  padding-bottom 27%
  .swiper-img
    width 100%
</style>
