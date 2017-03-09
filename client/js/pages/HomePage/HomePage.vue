<style scoped lang="scss" src="./HomePage.scss"></style>

<template>
  <div class="page">

    <div is="SidebarContainer"
         class="sidebar" >
    </div>

    <div>hello! world</div>

    <div class="main">
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

  </div>
</template>

<script>
import Card from 'components/Card'
import InfoBox from 'components/InfoBox'
import Counter from 'components/Counter'
import SidebarContainer from 'containers/SidebarContainer'
import ExplorePanel from 'components/ExplorePanel'

// TODO: Implement page builder
export default {
  created () {
    console.log('created Home')
  },
  components: {
    Card,
    Counter,
    SidebarContainer,
    InfoBox,
    ExplorePanel,
  },
  props: {
    test: { type: String, default: 'nothing!' }
  }
}
</script>
