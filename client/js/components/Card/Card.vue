<style scoped lang="scss" src="./Card.scss"></style>

<template>

  <div class="card component">

    <div class="component-pad">
      <div class="header">{{ header }}</div>
      <div class="formula-box">
        <App src="static/icon-hearthstone.png"></App>
        <Icon class="plus" type="plus"></Icon>
        <App src="static/icon-hearthstone.png"></App>
      </div>
      <div class="cardAction">
          <div class="card-label">If When
              <ifWhen
              >
              </ifWhen>
          </div>

          <div class="card-label">Do what
              <doWhat
                filter="wow"
              >
              </doWhat>
          </div>
      </div>

      <div class="actions">
        <div class="component-pad">
          <div class="action-button">Share</div>
          <div class="action-button">Bip</div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
  import App from 'components/App'
  import Icon from 'components/Icon'
  import ifWhen from 'components/ifWhen'
  import doWhat from 'components/doWhat'

  export default {
    props: {
      header: { type: String, default: null },
    },
    components: {
      App,
      Icon,
      ifWhen,
      doWhat,
    }
  }
</script>
