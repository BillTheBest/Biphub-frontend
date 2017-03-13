<style scoped lang="scss" src="./App.scss"></style>

<template>
  <div class="component"
       v-on:click="onClick" >
    <div class="app-icon">
      <img v-bind:src="src">
    </div>
    <div class="app-label"
         v-if="label" >
      {{ label }}
    </div>
  </div>
</template>

<script>
  export default {
    props: {
    	src: { type: String, default: 'N/A' },
    	label: { type: String, default: null },
    },
    methods: {
    	onClick() {
    		this.$emit('click')
      }
    }
  }
</script>
