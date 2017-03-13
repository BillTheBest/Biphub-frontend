<style scoped lang="scss" style="./Suggestion.scss"></style>

<template>
  <div class="component">
    <div class="component-pad">
      <div class="header"></div>
      <div>

      </div>
    </div>
  </div>
</template>

<script>
  import App from '../App'
  export default {
    props: {
    	colour: { type: String, default: 'blue' },
      header: { type: String, default: 'N/A' },
    },
    components: {
    	App,
    }
  }
</script>
