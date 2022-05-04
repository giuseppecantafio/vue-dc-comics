<template>
  <div>
    <div class="footer-top">
      <div class="footer-top-wrapper">
        <ul>
          <li v-for="(item, index) in footerTopLiElm" :key="index">
            <div class="img-wrapper">
              <img :src="item.immagine" alt="immagine" />
            </div>
            <span class="text-container">{{ item.testo }}</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppMain",
  data() {
    return {
      footerTopLiElm: [
        {
          immagine: require("../assets/img/buy-comics-digital-comics.png"),
          testo: "Digital comics",
        },
        {
          immagine: require("../assets/img/buy-comics-merchandise.png"),
          testo: "Dc merchandise",
        },
        {
          immagine: require("../assets/img/buy-comics-shop-locator.png"),
          testo: "Subscription",
        },
        {
          immagine: require("../assets/img/buy-comics-subscriptions.png"),
          testo: "Comic shop locator",
        },
        {
          immagine: require("../assets/img/buy-dc-power-visa.svg"),
          testo: "Dc power Visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
@import "../style/generals";

.footer-top {
  height: 160px;
  width: 100%;
  background-color: $bg-footer-top;

  .footer-top-wrapper {
    width: 75%;
    margin: 0 auto;
  }
  ul {
    @include inline-ul;
    line-height: 160px;
    vertical-align: middle;
    justify-content: space-around;
  }
  .img-wrapper {
    margin-top: 20px;
    width: 50px;
    height: 50px;
  }
  img {
    @include img-fit;
  }
  li {
    @include inline-li;
    display: flex;
  }
  .text-container {
    color: $light-color;
    padding-left: 5px;
  }
}
</style>
