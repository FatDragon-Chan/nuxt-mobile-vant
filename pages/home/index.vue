<template>
  <div>
    <searchBar />
    <mobileTemplate />
  </div>
</template>

<script>
  import searchBar from '~/components/SearchBar'
  import mobileTemplate from '~/pages/home/mobileTemplate'
  export default {
    name: 'Home',
    components: {
      mobileTemplate,
      searchBar,
    },
    layout: 'hasTabsView',
    data() {
      return {}
    },
  }
</script>

<style scoped></style>
