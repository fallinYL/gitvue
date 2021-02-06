<template>
  <div class='wrapper'>
    <swiper :options="swiperOptions">
      <swiper-slide v-for="item of list" :key="item.id">
         <img class="swiper-img" :src="item.imgUrl" >
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
   </swiper>
  </div>
</template>

<script>
import picbg from './1.png'
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        loop: true
      },
      list: [{
        id: '001',
        imgUrl: picbg
      },
      {
        id: '002',
        imgUrl: require('./1.png')
      }]
    }
  }
}
</script>

<style lang='stylus' scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background:#fff
  .wrapper
    overflow:hidden
    width:100%
    height:0
    padding-bottom:31.25%
    background :#eee
    .swiper-img
      width:100%

</style>
