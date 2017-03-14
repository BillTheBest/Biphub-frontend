<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <BasePage>
    <div class="base-main-width">
      <div>
        <Card title="test"
              link="http://naver.com"
              writer_name="Will Smith"
              crdate="2017-03-03"
              bgColor="gray"
        ></Card>

        <ExplorePanel v-on:onAppClick="onAppClick"
        ></ExplorePanel>
      </div>
    </div>
  </BasePage>
</template>

<script>
import BasePage from '../Base'
import InfoBox from 'components/InfoBox'
import ExplorePanel from 'components/ExplorePanel'
import Card from 'components/Card'

// TODO: Implement page builder
export default {
  components: {
    BasePage,
    Card,
    InfoBox,
    ExplorePanel,
    Card
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
