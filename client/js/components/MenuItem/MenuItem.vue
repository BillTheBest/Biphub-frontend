<style scoped lang="scss" src="./MenuItem.scss"></style>

<template>
  <div class="component">
    <div v-bind:class="direction">
      <Icon class="icon"
            v-bind:type="iconType"
      ></Icon>
      <div class="label">{{ label }}</div>
    </div>
  </div>
</template>

<script>
  import Icon from 'components/Icon'

  export default {
    props: {
      iconType: { type: String, default: null },
      label: { type: String, default: null },
      flexDirection: { type: String, default: 'column' },
    },
    components: {
      Icon,
    },
    computed: {
      /**
       * Decides flex direction
       * TODO: Implement strings used in this function in constants
       * @returns {string}
       */
    	direction() {
    		let baseStyle = 'component-pad'
    		switch (this.flexDirection) {
          case 'column-reverse':
          	return `${baseStyle} component--column-reverse`
          case 'row':
          	return `${baseStyle} component--row`
          case 'row-reverse':
          	return `${baseStyle} component--row-reverse`
          default:
            return `${baseStyle} component--column`
        }
      }
    },
  }
</script>
