<template>
  <div id="app">
    <BaseHeader></BaseHeader>
    <BaseMain></BaseMain>
    <BaseFooter></BaseFooter> 
  </div>
</template>

<script>
import BaseHeader from './components/header/BaseHeader.vue';
import BaseMain from './components/main/BaseMain.vue';
import BaseFooter from './components/footer/BaseFooter.vue';

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';

#app {}
</style>
