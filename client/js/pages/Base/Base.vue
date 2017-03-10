<style scoped lang="scss" src="./Base.scss"></style>

<template>
  <div class="page">

    <div is="SidebarContainer"
         class="sidebar" >
    </div>

    <div class="main">

      <div is="TopbarContainer"
           class="topbar" >
      </div>

      <slot class="base-main-width"></slot>

    </div>

  </div>
</template>

<script>
  import TopbarContainer from 'containers/TopbarContainer'
  import SidebarContainer from 'containers/SidebarContainer'
  export default {
    components: {
      TopbarContainer,
      SidebarContainer,
    }
  }
</script>
