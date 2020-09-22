<template>
  <div>
    <header-content></header-content>
    <swiper-content></swiper-content>
  </div>
</template>

<script>
import HeaderContent from '@/pages/home/components/Header'
import SwiperContent from '@/pages/home/components/Swiper'

export default {
  name: 'Home',
  components: {
    HeaderContent,
    SwiperContent
  }
}
</script>

<style scoped>

</style>
