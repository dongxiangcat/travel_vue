<template>
  <div class="guess">
    <div class="title">
      <img class="title-icon" src="http://img1.qunarzz.com/piao/fusion/1711/89/ebc329f16c55bb02.png">
      <span class="title-content">猜你喜欢</span>
    </div>
    <div class="content">
      <ul>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>

        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>
        <li class="content-item border-bottom">
        <div class="item-img">
          <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
        </div>
        <div class="item-content">
          <div class="item-name">奥林匹克公园</div>
          <div class="item-comment">637条评论</div>
          <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
            起
            <span class="location">朝阳区</span>
          </div>
        </div>
      </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>
        <li class="content-item border-bottom">
          <div class="item-img">
            <img src="http://img1.qunarzz.com/sight/p0/1804/1a/1a48cc20b0d6ed44a3.img.jpg_200x200_32e22bed.jpg">
          </div>
          <div class="item-content">
            <div class="item-name">奥林匹克公园</div>
            <div class="item-comment">637条评论</div>
            <div class="item-info">
              <span class="price">
                ¥
                <em class="number">165</em>
              </span>
              起
              <span class="location">朝阳区</span>
            </div>
          </div>
        </li>

      </ul>
    </div>
    <div class="more border-bottom">查看所有产品</div>
  </div>
</template>

<script>
export default {
  name: 'HomeGuess'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
.guess
  width: 100%
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
  .content
    padding 0 .24rem
    .content-item
      display flex
      padding .2rem 0
      .item-img
        img
          width 2rem
          height 2rem
      .item-content
        flex 1
        margin-left .24rem
        .item-name
          margin-top:.26rem
          font-size .32rem
          line-height .44rem
          height .44rem
          color #212121
        .item-comment
          margin-top .14rem
          height .34rem
          color #616161
        .item-info
          margin-top .22rem
          font-size .24rem
          line-height .4rem
          color: #616161
          position relative
          .price
            color: #ff8300
            font-size .24rem
            .number
              font-size .4rem
          .location
            right 0
            position absolute
  .more
    height .9rem
    line-height .9rem
    text-align center
    color $bgColor
    font-size .28rem

</style>
