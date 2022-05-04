<template>
  <div>
    <div class="footer-bottom">
      <div class="fb-wrapper">
        <div class="fb-left">
          <span class="sign-up">Sign-up now!</span>
        </div>
        <div class="fb-right">
          <span class="text-container">Follow us</span>
          <ul>
            <li v-for="(item, index) in icons" :key="index">
              <img :src="item.immagine" />
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooterBot",
  data() {
    return {
      icons: [
        {
          piattaforma: "facebook",
          immagine: require("../assets/img/footer-facebook.png"),
        },
        {
          piattaforma: "twitter",
          immagine: require("../assets/img/footer-twitter.png"),
        },
        {
          piattaforma: "youtube",
          immagine: require("../assets/img/footer-youtube.png"),
        },
        {
          piattaforma: "pinterest",
          immagine: require("../assets/img/footer-pinterest.png"),
        },
        {
          piattaforma: "periscope",
          immagine: require("../assets/img/footer-periscope.png"),
        },
      ],
    };
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
      display: flex;
      align-items: center;
      gap: 40px;
    }
    .fb-right {
      justify-content: flex-end;
    }
  }
  .sign-up {
    padding: 10px 5px;
    margin: 2px;
    border: 2px solid $color-border-footer-bot-sign-up-now;
    text-transform: uppercase;
    color: white;
  }
  .text-container {
    text-transform: uppercase;
    color: $color-footer-bot-follow-us;
  }
  ul {
    @include inline-ul;
    line-height: 0 !important;
    gap: 10px;
  }
  li {
    @include inline-li;
  }
}
</style>
