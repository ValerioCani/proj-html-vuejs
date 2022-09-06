<template>
  <div id="app">
    <HeaderMaster/>
    <MainMaster/>
    <FooterMaster/>
  </div>
</template>

<script>
import HeaderMaster from './components/HeaderMaster.vue'
import MainMaster from './components/MainMaster.vue'
import FooterMaster from './components/FooterMaster.vue'

export default {
  name: 'App',
  components: {
    HeaderMaster,
    MainMaster,
    FooterMaster,
  }
}
</script>
<style lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.css';
@import './assets/styles/general.scss';
@import './assets/styles/var.scss';
</style>
