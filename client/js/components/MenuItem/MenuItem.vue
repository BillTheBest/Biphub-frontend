<style scoped lang="scss" src="./MenuItem.scss"></style>

<template>
  <div class="component">
    <Icon></Icon>
    <div>{{ label }}</div>
  </div>
</template>

<script>
  import Icon from 'components/Icon'
  export default {
    components: {
      Icon,
    },
    props: {
    	icon: { type: String, default: null },
      label: { type: String, default: null, },
    }
  }
</script>
