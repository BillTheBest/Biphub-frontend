<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <BasePage>
    <div class="base-main-width">
      <div>
        <ExplorePanel v-on:onAppClick="onAppClick"
        ></ExplorePanel>
      </div>
    </div>
  </BasePage>
</template>

<script>
import BasePage from '../Base'
import Card from 'components/Card'
import InfoBox from 'components/InfoBox'
import ExplorePanel from 'components/ExplorePanel'

// TODO: Implement page builder
export default {
  components: {
    BasePage,
    Card,
    InfoBox,
    ExplorePanel,
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
