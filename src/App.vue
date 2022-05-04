<template>
  <div id="app">
    <AppHeader/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    AppHeader
  }
}
</script>

<style lang="scss">
@import './style/generals';
@import './style/variables';

.debug{
  border: 1px solid black;
}
</style>
