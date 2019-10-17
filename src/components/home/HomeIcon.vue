<template>
<div class="home-icons border-bottom">
  <div class="home-icons-content">
    <swiper :options="swiperOption" ref="swiperTop">
      <swiper-slide>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png" class="icon-img-content">
        </div>
        <p class="icon-desc">景点门票</p>
      </div>

      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/6c/9e54a8540fee0102.png" class="icon-img-content">
        </div>
        <p class="icon-desc">故宫</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png" class="icon-img-content">
        </div>
        <p class="icon-desc">北京必游</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png" class="icon-img-content">
        </div>
        <p class="icon-desc">水上乐园</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png" class="icon-img-content">
        </div>
        <p class="icon-desc">一日游</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/67/9a1678221b8e0e02.png" class="icon-img-content">
        </div>
        <p class="icon-desc">古北水镇</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/fa/2548667cb6e902.png" class="icon-img-content">
        </div>
        <p class="icon-desc">动植物园</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png" class="icon-img-content">
        </div>
        <p class="icon-desc">赏红叶</p>
      </div>
      </swiper-slide>

      <swiper-slide>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://img1.qunarzz.com/piao/fusion/1803/ab/6f7d6e44963c9302.png" class="icon-img-content">
        </div>
        <p class="icon-desc">泡温泉</p>
      </div>
      <div class="home-icon-item">
        <div class="icon-img">
          <img src="http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20197/bf88c62458044ca2ef9d733690eef3fc.png" class="icon-img-content">
        </div>
        <p class="icon-desc">优惠券</p>
      </div>
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
  <!-- swiper2 Thumbs -->
  <div class="home-icons-pagination">
    <swiper :options="swiperOptionThumbs" class="gallery-thumbs" ref="swiperThumbs">
      <swiper-slide class="slide-thumb"></swiper-slide>
      <swiper-slide class="slide-thumb"></swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</div>
</template>

<script>
import  { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'HomeIcon',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      swiperOption: {
        loop: false,
        spaceBetween: 5,
      },

      swiperOptionThumbs: {
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        }
      }
    }
  },
  mounted() {
    this.$nextTick(() => {
      const swiperTop = this.$refs.swiperTop.swiper
      const swiperThumbs = this.$refs.swiperThumbs.swiper
      swiperTop.controller.control = swiperThumbs
      swiperThumbs.controller.control = swiperTop
    })
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl'
.home-icons-pagination >>> .swiper-pagination-bullets
  bottom: 0
.home-icons-pagination >>> .swiper-pagination-bullet
  width .12rem
  height .12rem
.home-icons-pagination >>> .swiper-pagination-bullet-active
  background-color $bgColor
.home-icons
  padding-top .1rem
  background-color white
  .home-icons-pagination
    width 100%
    padding .2rem 0 .1rem
    .slide-thumb
      height .2rem
  .home-icons-content
    width 100%
    padding-bottom 39%
    height 0
    overflow hidden
    .home-icon-item
      width 25%
      height 0
      float left
      padding-bottom 19%
      position relative
      overflow hidden
      .icon-img
        position absolute
        left 0
        top: 0
        right 0
        bottom .44rem
        box-sizing border-box
        padding .02rem
        .icon-img-content
          display block
          margin 0 auto
          height:100%
      .icon-desc
        position: absolute
        bottom: 0
        left 0
        right 0
        line-height .44rem
        height:.44rem
        color #333
        text-align center
        font-size .28rem
</style>
