<template>
  <van-tabbar v-model="active">
    <van-tabbar-item icon="home-o">首页</van-tabbar-item>
    <van-tabbar-item icon="search">分类</van-tabbar-item>
    <van-tabbar-item icon="friends-o">购物车</van-tabbar-item>
    <van-tabbar-item icon="setting-o">个人中心</van-tabbar-item>
  </van-tabbar>
</template>

<script>
  export default {
    name: 'TabsView',
    data() {
      return {
        active: '',
      }
    },
  }
</script>

<style scoped></style>
