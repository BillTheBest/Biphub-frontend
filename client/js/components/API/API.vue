<style scoped lang="scss" src="./API.scss"></style>

<template>
  <div class="component">
    <div class="api-icon">
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
    	src: { type:String, default: 'N/A' },
    	label: { type: String, default: 'N/A' },
    }
  }
</script>
