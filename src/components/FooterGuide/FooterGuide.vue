<template>
  <footer class="footer_guide border-1px">
    <!-- <a href="javascript:;" class="guide_item on">
    <span class="item_icon">
    <i class="iconfont icon-food"></i>
    </span>
    <span>外卖</span>
    </a> -->
    <div class="guide_item" @click="goto('/msite')" :class="{on: isCurrent('/msite')}">
    <span class="item_icon">
    <i class="iconfont"><svg t="1570300129610" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="4038" width="22" height="22"><path d="M989.6 484C884.8 376 777.6 266.4 673.6 161.6l-75.2-76C573.6 60 543.2 48 507.2 49.6c-32 1.6-58.4 15.2-88 44.8-86.4 88-173.6 177.6-258.4 264-39.2 40-78.4 79.2-116.8 119.2l-3.2 3.2c-5.6 5.6-11.2 11.2-15.2 16.8-16.8 22.4-16 44 0 63.2 17.6 20 39.2 22.4 62.4 8 5.6-4 11.2-8 19.2-13.6 3.2-2.4 7.2-5.6 12-8.8v135.2c0 54.4 0 110.4 0.8 165.6 0.8 82.4 46.4 127.2 130.4 128.8 20.8 0 42.4 0.8 63.2 0.8 20.8 0 42.4 0 64-0.8 53.6-0.8 68-14.4 68.8-67.2 0.8-20.8 0-42.4 0-63.2v-58.4c0-9.6 1.6-18.4 3.2-28.8 0.8-4 1.6-8.8 1.6-13.6h110.4c20.8 0 41.6 0.8 62.4-0.8 32-1.6 52.8-22.4 51.2-49.6-1.6-26.4-21.6-43.2-51.2-44-68-0.8-140-1.6-226.4 0-28.8 0-46.4 17.6-47.2 48-0.8 24.8-0.8 50.4-0.8 75.2v102.4c-7.2 0.8-12.8 0.8-19.2 1.6-12.8 0.8-23.2 1.6-34.4 1.6-35.2 0-56.8-1.6-68.8-13.6-11.2-11.2-13.6-32.8-13.6-66.4V689.6c0-69.6 0-140.8-0.8-211.2-0.8-24.8 7.2-43.2 25.6-61.6 46.4-46.4 93.6-94.4 138.4-140 27.2-28 55.2-56 83.2-84 23.2-23.2 38.4-36 53.6-36 14.4 0 30.4 12.8 52 35.2 68.8 69.6 138.4 140.8 206.4 209.6l131.2 133.6c3.2 3.2 5.6 6.4 8.8 9.6 8.8 9.6 17.6 19.2 28 24 13.6 6.4 35.2 9.6 47.2 2.4 12-6.4 23.2-26.4 23.2-41.6 0.8-16.8-10.4-35.2-20.8-45.6z" p-id="4039" ></path><path d="M906.4 760v-0.8h-0.8v-32c0-25.6 0.8-51.2-0.8-76.8-1.6-28.8-20-47.2-46.4-47.2-25.6 0-42.4 16.8-46.4 47.2-1.6 9.6-1.6 20-1.6 30.4v129.6c-0.8 56-11.2 66.4-67.2 68h-38.4c-25.6 0-52 0-76.8 2.4-14.4 1.6-33.6 16.8-40 31.2-5.6 12 0.8 36 9.6 45.6 9.6 10.4 29.6 15.2 44.8 16 24 0.8 48 1.6 71.2 1.6 24.8 0 47.2-0.8 67.2-0.8 77.6-1.6 123.2-47.2 126.4-124.8 0.8-20 0.8-40.8 0-60.8-0.8-10.4-0.8-19.2-0.8-28.8z" p-id="4040"></path></svg></i>
    </span>
    <span>首页</span>
    </div>
    <div class="guide_item" @click="goto('/order')" :class="{on: isCurrent('/order')}">
    <span class="item_icon">
    <i class="iconfont icon-single"></i>
    </span>
    <span>课表</span>
    </div>
    <div class="guide_item" @click="goto('/profile')" :class="{on: isCurrent('/profile')}">
    <span class="item_icon">
    <i class="iconfont icon-user"></i>
    </span>
    <span>我的</span>
    </div>
  </footer>
</template>

<script>
export default {
  methods: {
    goto (path) {
      this.$router.replace(path)
    },
    isCurrent (path) {
      // console.log(this.$route.path)
      return this.$route.path === path
    }
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
/*引入公共样式*/
@import "../../common/stylus/mixins.styl"
.footer_guide
  // 顶部有白色的边框
  top-border-1px(#e4e4e4)
  position fixed
  z-index 100
  left 0
  right 0
  bottom 0
  background-color #fff
  width 100%
  height 50px
  display flex
  .guide_item
    display flex
    flex 1
    text-align center
    flex-direction column
    align-items center
    margin 5px
    color #999999
    &.on
      color #F3A033
      fill #F3A033
    span
      font-size 12px
      margin-top 2px
      margin-bottom 2px
      .iconfont
        font-size 22px
</style>
