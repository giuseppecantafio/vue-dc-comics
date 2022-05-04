<template>
  <div>
    <div class="footer-bottom">
      <div class="fb-wrapper">
        <div class="fb-left">
  
        </div>
        <div class="fb-right">

        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooterBot",
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
@import "../style/generals";
.footer-bottom {
  width: 100%;
  height: 100px;
  background-color: $bg-footer-bot;

  .fb-wrapper {
    width: 80%;
    height: 100%;
    margin: 0 auto;
    display: flex;

    .fb-left,
    .fb-right {
      width: 50%;
      height: 100%;
    }
    
  }
}

</style>
