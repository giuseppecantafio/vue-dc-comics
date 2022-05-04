<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppFooterTop />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooterTop from "./components/AppFooterTop.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooterTop,
  },
};
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/variables";

.debug {
  border: 1px solid black;
}
</style>
