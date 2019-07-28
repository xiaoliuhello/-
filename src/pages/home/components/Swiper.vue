<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperList" :key="item.id">
          <img class="swiper-img" :src="item.imgUrl">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://source.qunarzz.com/site/images/wns/20190725_dujia_750x192_11555.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://source.qunarzz.com/site/images/wns/20190722_dujia_homepage_750x192_2.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active{
    background: #fff !important;
  }
.swiper-img{
  width:100%;
  /*height:4rem;*/
}
  .wrapper{
    width:100%;
    height:0;
    padding-bottom: 25.7%;

    background #eee;
    overflow hidden;
  }

</style>
