<style scoped lang="scss" src="./InfoBox.scss"></style>

<template>
  <div class="component">

    <div class="values">
      <div class="values-heading">{{ value }}</div>
      <div>
        <Icon v-bind:type="iconType"
        ></Icon>
      </div>
    </div>

    <div class="description">{{ description }}</div>

  </div>
</template>

<script>
  import Icon from 'components/Icon'
  export default {
  	components: [
      Icon
    ],
    props: {
    	value: { type: String, default: 'N/A' },
    	iconType: { type: String, default: 'home' },
      description: { type: String, default: 'N/A' },
    },
  }
</script>
