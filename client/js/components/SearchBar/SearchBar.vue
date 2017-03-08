<style scoped lang="scss" src="./SearchBar.scss"></style>

<template>
  <div class="search-bar">
    <Icon type="search"
          class="icon" ></Icon>
    <input placeholder="Search for any app name..."
           class="input" >
  </div>
</template>

<script>
  import Icon from 'components/Icon'
  export default {
    components: {
    	Icon,
    }
  }
</script>
