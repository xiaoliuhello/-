<template>
  <div>
      <div class="header">
        <div class="header-left">
          <span class="iconfont">&#xe624;</span>
        </div>
        <div class="header-input">
          <span class="iconfont">&#xe632;</span>
          输入城市/景点/游玩
        </div>
        <div class="header-right">
          城市
          <span class="iconfont arrow-iconfont">&#xea81;</span>
        </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
@import "~styles/varibles.styl"
  .header{
    display: flex ;
    line-height:.86rem;
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
  }
  .arrow-iconfont{
    font-size .24rem;
    margin-left -.04rem
  }
</style>
