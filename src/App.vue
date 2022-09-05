<template>
  <div id="app">
    <MasterHeader/>
    <MasterMain/>
    <MasterFooter/>
  </div>
</template>

<script>
import MasterHeader from './components/MasterHeader.vue'
import MasterMain from './components/MasterMain.vue'
import MasterFooter from './components/MasterFooter.vue'

export default {
  name: 'App',
  components: {
    MasterHeader,
    MasterMain,
    MasterFooter,
  }
}
</script>
<style lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.css';
@import './assets/styles/general.scss';
@import './assets/styles/var.scss';
</style>
