<style scoped lang="scss" src="./ExplorePanel.scss"></style>

<template>
  <div class="explore-panel">
    <div class="component-pad">
      <SearchBar></SearchBar>
    </div>
  </div>
</template>

<script>
  import Icon from 'components/Icon'
  import SearchBar from 'components/SearchBar'

  export default {
    components: {
    	Icon,
      SearchBar,
    }
  }
</script>
