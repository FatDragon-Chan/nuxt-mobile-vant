<template>
  <div id="container">
    <!-- 轮播组件 -->
    <swiper />

    <!-- 导航栏组件 -->

    <!-- 楼层样式 一 -->
    <!-- 楼层样式 二 -->
    <!-- 为你推荐组件 -->
    <!-- 为你推荐组件 -->
  </div>
</template>

<script>
  import swiper from '~/pages/home/swiper'
  export default {
    name: 'MobileTemplate',
    components: {
      swiper,
    },
  }
</script>

<style scoped></style>
