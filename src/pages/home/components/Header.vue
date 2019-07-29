<template>
  <div>
      <div class="header">
        <div class="header-left">
          <div class="iconfont back-icon">&#xe624;</div>
        </div>
        <div class="header-input">
          <span class="iconfont">&#xe632;</span>
          输入城市/景点/游玩
        </div>
        <router-link to="/city">
          <div class="header-right">
            {{this.city}}
            <span class="iconfont arrow-iconfont">&#xea81;</span>
          </div>
        </router-link>
      </div>
  </div>
</template>

<script>

export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
@import "~styles/varibles.styl"
  .header{
    display: flex ;
    line-height: $headerHeight;
    background :$bgColor;
    color #fff;
  }
  .header-left{
    width :.64rem;
    float: left ;
  }
  .header-input{
    flex :1;
    margin-top .12rem;
    height .64rem;
    margin-left .12rem;
    background:#fff;
    border-radius :.1rem;
    color #ccc;
    height .64rem;
    padding-left .2rem
    float left ;
    text-align left ;
    line-height .64rem;
  }
  .header-right{
    width :1.24rem;
    float :right ;
    text-align :center;
    color #fff;
  }
  .arrow-iconfont{
    font-size .24rem;
    margin-left -.04rem
  }
</style>
