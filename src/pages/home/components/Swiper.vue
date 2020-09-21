<template>
  <div class="swiper">
    <img src="" alt="">
    <swiper :options="swiperOption">
      <swiper-slide><img src="http://travel.qunar.com/travelbook/note/7618438"></swiper-slide>
      <swiper-slide><img src="http://travel.qunar.com/travelbook/note/7618370"></swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'SwiperContent',
  data () {
    return {
      swiperOption: {
        // some swiper options/callbacks
        // 所有的参数同 swiper 官方 api 参数
        // ...
      }
    }
  }
}
</script>
<style scoped>
  .swiper{

  }
</style>
