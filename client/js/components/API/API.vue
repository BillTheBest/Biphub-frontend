<style scoped lang="scss" src="./API.scss"></style>

<template>
  <div class="component"
       v-on:click="onClick">
    <div class="api-icon" v-bind:style="{border: border, backgroundColor: backgroundColor, borderRadius:borderRadius}">
      <img v-bind:src="src">
    </div>
    <div class="api-label">
      {{ label }}
    </div>
  </div>
</template>

<script>
  export default {
    props: {
    	src: { type: String, default: 'N/A' },
    	label: { type: String, default: 'N/A' },
        border: { type: String, default: '2px solid $color-light-blue' },
        backgroundColor: { type: String, default: 'N/A' },
        borderRadius: { type: String, default: '50%' },
    },
    methods: {
    	onClick() {
    		console.log('clicked!')
    		this.$emit('click')
      }
    }
  }
</script>
