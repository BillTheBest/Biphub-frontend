<style scoped lang="scss" src="./ExplorePanel.scss"></style>

<template>
  <div class="explore-panel">
    <div class="component-pad">
      <SearchBar></SearchBar>
    </div>

    <div class="component-pad api-list">
      <API label="Discord"
           src="static/icon-discord.png"
      ></API>
      <API label="Dota 2"
           src="static/icon-dota2.png"
      ></API>
      <API label="Gmail"
           src="static/icon-gmail.png"
      ></API>
      <API label="Hearthstone"
           src="static/icon-hearthstone.png"
      ></API>
      <API label="Minecraft"
           src="static/icon-minecraft.png"
      ></API>
      <API label="Overwatch"
           src="static/icon-overwatch.png"
      ></API>
      <API label="Team Fortress2"
           src="static/icon-tf2.png"
      ></API>
      <API label="WoW"
           src="static/icon-wow.png"
      ></API>

    </div>
  </div>
</template>

<script>
  import API from 'components/API'
  import Icon from 'components/Icon'
  import SearchBar from 'components/SearchBar'

  export default {
    components: {
    	Icon,
      SearchBar,
      API,
    }
  }
</script>
