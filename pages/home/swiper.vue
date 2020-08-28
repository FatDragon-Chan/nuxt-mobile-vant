<template>
  <van-swipe :autoplay="options.autoplay" :height="options.height" :style="`border-radius: ${options.borderRadius}px; overflow:hidden`">
    <van-swipe-item v-for="(advert, index) in adverts" :key="index">
      <van-image :height="options.height" :lazy-load="options.lazyLoad" :fit="options.fit" :src="advert.image" @click="goToDetail(advert)" />
    </van-swipe-item>
  </van-swipe>
</template>

<script>
  export default {
    props: {
      options: {
        type: Object,
        default: () => {
          return {
            height: 168,
            borderRadius: 12,
            autoplay: 3000,
            fit: 'cover',
            lazyLoad: true,
          }
        },
      },
      adverts: {
        type: Array,
        default: () => {
          return [
            {
              image: 'https://wanshunfu-1301582899.cos.ap-guangzhou.myqcloud.com//11111/e3911e4b01558384427e2e2a8dd91d71H5lb3.png',
            },
            {
              image: 'https://wanshunfu-1301582899.cos.ap-guangzhou.myqcloud.com//11111/254b365d6eb9564c1a3858b7e167d942H5lb1.png',
            },
            {
              image: 'https://wanshunfu-1301582899.cos.ap-guangzhou.myqcloud.com//11111/28ff0d93f0fb4874fa199c1fbbd9b0f5H5lb2.png',
            },
          ]
        },
      },
    },
    name: 'swiper',
    data() {
      return {}
    },
    methods: {
      goToDetail(advert) {
        console.log(advert)
      },
    },
  }
</script>

<style scoped></style>
