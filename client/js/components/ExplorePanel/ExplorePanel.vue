<style scoped lang="scss" src="./ExplorePanel.scss"></style>

<template>
  <div class="component">
    <div class="component-pad">
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
