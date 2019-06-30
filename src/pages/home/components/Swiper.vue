<template>
    <div class="swiper">
        <swiper  :options="swiperOption" ref="mySwiper">
            <swiper-slide v-for="item of swiperList" :key=item.id>
                <img class="img-swiper" :src="item.src">
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
      swiperList: [{
        id: '001',
        src: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/9f581f130d65e97c01301661e1e4116f.jpg_750x200_e5b996c3.jpg'
      }, {
        id: '002',
        src: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/818f6cc784ae6669b74bbbb255414a53.jpg_750x200_66ca5873.jpg'
      }, {
        id: '003',
        src: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/b48d1ce6662a905d993635b4e28ff089.jpg_750x200_1c00b2f0.jpg'
      }],
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
    .swiper >>> .swiper-pagination-bullet-active
        background: #ffffff
    .swiper
        width: 100%
        height: 0
        overflow: hidden
        padding-bottom: 26.8%
        .img-swiper
            width: 100%
</style>
