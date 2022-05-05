<template>
  <div id="app">
    <AppHeader />
    <AppJumbotron />
    <AppMain />
    <AppFooterTop />
    <AppFooterMid />
    <AppFooterBot />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbotron from "./components/AppJumbotron.vue"
import AppMain from "./components/AppMain.vue";
import AppFooterTop from "./components/AppFooterTop.vue";
import AppFooterMid from "./components/AppFooterMid.vue";
import AppFooterBot from "./components/AppFooterBot.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFooterTop,
    AppFooterMid,
    AppFooterBot
  },
  data() {
    return {};
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
