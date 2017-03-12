<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <BasePage>
    <div class="base-main-width">
      <div>
        <ExplorePanelContainer v-on:onAppClick="onAppClick"
        ></ExplorePanelContainer>
      </div>
    </div>
  </BasePage>
</template>

<script>
import BasePage from '../Base'
import ExplorePanelContainer from 'containers/ExplorePanelContainer'
import Card from 'components/Card'
import InfoBox from 'components/InfoBox'

// TODO: Implement page builder
export default {
  components: {
    BasePage,
    Card,
    InfoBox,
    ExplorePanelContainer,
  },
  props: {
    test: { type: String, default: 'nothing!' }
  },
  methods: {
  	onAppClick() {
  		console.log('testing!')
      // this.$router.
    }
  }
}
</script>
