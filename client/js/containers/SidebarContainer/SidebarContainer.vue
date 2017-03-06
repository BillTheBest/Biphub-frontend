<style scoped lang="scss" src="./SidebarContainer.scss"></style>

<template>
  <div class="container">
    <LogoText></LogoText>
    <UserProfile class="side-user-profile"
                 photo="/static/profile-menu-image.png"
                 name="jason"
                 role="developer"
    ></UserProfile>
    <MenuItem class="component-side"
    ></MenuItem>
    <MenuItem class="component-side"
    ></MenuItem>
    <MenuItem class="component-side"
    ></MenuItem>
  </div>
</template>

<script>
  import LogoText from 'components/LogoText'
  import UserProfile from 'components/UserProfile'
  import MenuItem from 'components/MenuItem'

  export default {
    components: {
      LogoText,
      UserProfile,
      MenuItem,
    }
  }
</script>
