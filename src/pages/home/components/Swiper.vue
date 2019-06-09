<template>
  <div class="wapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" />
      </swiper-slide>
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
        imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/5a613f91d1e95a8442fa128957565be8.jpg_750x200_7ad50d73.jpg'
      }, {
        id: '0002',
        imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/f31e841aa64b60e5f5e8b14b8ba92825.jpg_750x200_0baeb58b.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wapper >>> .swiper-pagination-bullet-active
      background: #fff
  .wapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 27%
    background: #eee
    .swiper-img
      width: 100%
</style>
