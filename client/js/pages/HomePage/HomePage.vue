<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <BasePage>
    <div class="base-main-width">
      <div>
        <ExplorePanel></ExplorePanel>
      </div>

      <div class="info-row">
        <Card>
          <InfoBox value="1231244"
                   iconType="users"
                   description="User activity this month"
          ></InfoBox>
        </Card>
        <Card>
          <div>testzz</div>
        </Card>
        <Card>
          <div>testzz</div>
        </Card>
        <Card>
          <div>testzz</div>
        </Card>
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
  }
}
</script>
