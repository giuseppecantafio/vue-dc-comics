<template>
  <div>
    <div class="footer-mid">
      <div class="footer-mid-wrapper">
        <div class="fm-left">
          <ul>
            <li></li>
          </ul>
        </div>
        <div class="fm-right"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooterMid",
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
@import "../style/generals";
.footer-mid {
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
  width: 100%;

  .footer-mid-wrapper {
    width: 80%;
    height: 100%;
    margin: 0 auto;
    display: flex;

    .fm-left,
    .fm-right {
      width: 50%;
      height: 100%;
    }
    .fm-right {
      background-image: url("../assets/img/dc-logo-bg.png");
      background-repeat: no-repeat;
      background-size: cover;
      background-position: center;
    }
  }
}
</style>
