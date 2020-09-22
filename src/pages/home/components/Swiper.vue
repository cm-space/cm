<template>
  <div class="swiper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of banners" :key="item.id">
        <img class="swiper-img" :src="item.src">
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'SwiperContent',
  data () {
    return {
      banners: [
        {
          id: '2001',
          src: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1600767195406&di=eca8cfc691c1b817ad7d5516ac52f5b6&imgtype=0&src=http%3A%2F%2Fhbimg.huabanimg.com%2F074fec0acf549e60d27a42e56e96aca127e081fc1fd23-j63WXm_fw658'
        },
        {
          id: '2002',
          src: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1600767213097&di=c961d2e18496913a49fc07417ab73d92&imgtype=0&src=http%3A%2F%2Fhbimg.huabanimg.com%2F12791ec7c9655e6e5ca396b12ea221d10c672d4d23ced-RFH9Rs_fw658'
        }],
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true,
        autoplay: 2000
      }
    }
  }
}
</script>
<style lang="scss" scoped>
//.swiper >>> .swiper-pagination-bullet-active {
//  background: #ffffff;
//}
//
///*设置盒子初始化高度为图片的高宽比*/
//.swiper {
//  width: 100%;
//  height: 0;
//  padding-bottom: 36%;
//}
//
//.swiper-img {
//  width: 100%;
//}

.swiper {
  width: 100%;
  height: 0;
  padding-bottom: 36%;
  .swiper-img{
    width: 100%;
  }
}

</style>
