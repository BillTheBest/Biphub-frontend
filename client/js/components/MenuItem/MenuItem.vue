<style scoped lang="scss" src="./MenuItem.scss"></style>

<template>
  <div class="component">
    <div class="component-pad">
      <Icon v-bind:type="iconType"></Icon>
      <div class="label">{{ label }}</div>
    </div>
  </div>
</template>

<script>
  import Icon from 'components/Icon'

  export default {
    components: {
      Icon,
    },
    computed: {
    	direction() {

    }
    },
    props: {
    	iconType: { type: String, default: null },
      label: { type: String, default: null },
    }
  }
</script>
