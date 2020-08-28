<template>
  <div>
    <van-search v-model="searchValue" shape="round" show-action placeholder="请输入搜索关键词">
      <template #label>我是左侧内容</template>
      <template #left-icon>左侧图标</template>
      <template #action>
        <div>搜索</div>
      </template>
    </van-search>
  </div>
</template>

<script>
  export default {
    name: 'SearchBar',
    data() {
      return {
        searchValue: '',
      }
    },
  }
</script>

<style scoped></style>
