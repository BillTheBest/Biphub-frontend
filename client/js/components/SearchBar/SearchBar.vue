<style scoped lang="scss" src="./SearchBar.scss"></style>

<template>
  <div class="search-bar">
    <div class="search-bar-pad">
      <Icon type="search"
            class="icon" ></Icon>
      <input placeholder="Search for any app name..."
             class="input" >
    </div>
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
