<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppFooterTop />
    <AppFooterMid />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooterTop from "./components/AppFooterTop.vue";
import AppFooterMid from "./components/AppFooterMid.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooterTop,
    AppFooterMid,
  },
  data() {
    return {
    }
  }
};
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/variables";

.debug {
  border: 1px solid black;
}
</style>
