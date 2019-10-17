<template>
  <div class="hot">
    <div class="title">
      <img class="title-icon" src="http://img1.qunarzz.com/piao/fusion/1711/16/bfbb9874e8f11402.png">
      <span class="title-content">本周热门榜单</span>
      <a class="title-more">全部榜单</a>
    </div>
    <div class="content">
      <swiper :options="swiperOption">
        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>

        <swiper-slide>
          <a class="content-item">
            <div class="content-img">
              <img src="http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_250x250_0fc722c0.jpg">
            </div>
            <div class="content-name">故宫</div>
            <div class="content-desc">¥<em class="price">60</em>起</div>
          </a>
        </swiper-slide>
        <div class="swiper-scrollbar"   slot="scrollbar"></div>
      </swiper>
    </div>
  </div>
</template>
<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'HomeHot',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      swiperOption: {
        slidesPerView: 'auto',
        spaceBetween: 0,
        scrollbar: {
          el: '.swiper-scrollbar',
          hide: true,
          draggable: true,
          snapOnRelease: true,
          dragSize: 200
        }
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
  .hot >>> .swiper-wrapper
    padding-bottom .24rem
  .hot >>> .swiper-slide
    width 2.24rem
    &:last-child
      width 2.48rem
  .hot >>> .swiper-scrollbar-drag
    background-color #cacaca
  .hot
    width: 100%
    height: 3.9rem
    display flex
    flex-direction: column
    margin-top .3rem
    background-color white
    .title
      height .44rem
      line-height .44rem
      display flex
      padding .24rem 0 .26rem
      .title-icon
        width .3rem
        height .3rem
        margin-left .2rem
        display block
      .title-content
        font-size .32rem
        margin-left .08rem
        flex 1
      .title-more
        font-size .28rem
        margin-right .6rem
        color: #616161
    .content
      flex 1
      .content-item
        display flex
        flex-direction column
        float left
        margin-left .24rem
        .content-img
          img
            width 2rem
            height 2rem
        .content-name
          font-size .24rem
          line-height .32rem
          color: #212121
          text-align center
          margin-top .12rem
        .content-desc
          font-size .24rem
          line-height .32rem
          color: #616161
          text-align center
          .price
            font-size .28rem
            color #ff8300
</style>
