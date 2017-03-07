<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <div class="page">
    <div is="SidebarContainer"
         class="sidebar" >
    </div>
    <div class="main">
      test
    </div>
  </div>
</template>

<script>
import Counter from 'components/Counter'
import SidebarContainer from 'containers/SidebarContainer'

export default {
  created () {
    console.log('created Home')
  },
  components: {
    Counter,
    SidebarContainer,
  },
  props: {
    test: { type: String, default: 'nothing!' }
  }
}
</script>
