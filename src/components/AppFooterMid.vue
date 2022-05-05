<template>
  <div>
    <div class="footer-mid">
      <div class="footer-mid-wrapper">
        <div class="fm-left">
          <div>
            <h4>Dc comics</h4>
            <ul>
              <li v-for="(item, index) in dcComics" :key="index">
                {{ item.testo }}
              </li>
            </ul>
            <h4>Shop</h4>
            <ul>
              <li v-for="(item, index) in shop" :key="index">
                {{ item.testo }}
              </li>
            </ul>
          </div>
          <div>
            <h4>Dc</h4>
            <ul>
              <li v-for="(item, index) in dc" :key="index">
                {{ item.testo }}
              </li>
            </ul>
          </div>
          <div>
            <h4>Sites</h4>
            <ul>
              <li v-for="(item, index) in sites" :key="index">
                {{ item.testo }}
              </li>
            </ul>
          </div>
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
    return {
      dcComics: [
        {
          testo: "Characters",
          link: "",
          active: false
        },
        {
          testo: "Comics",
          link: "",
          active: false
        },
        {
          testo: "Movies",
          link: "",
          active: false
        },
        {
          testo: "TV",
          link: "",
          active: false
        },
        {
          testo: "Games",
          link: "",
          active: false
        },
        {
          testo: "Videos",
          link: "",
          active: false
        },
        {
          testo: "News",
          link: "",
          active: false
        },
      ],
      shop: [
        {
          testo: "Shop DC",
          link: "",
          active: false
        },
        {
          testo: "Shop DC Collectibles",
          link: "",
          active: false
        },
      ],
      dc: [
        {
          testo: "Terms of Use",
          link: "",
          active: false
        },
        {
          testo: "Privacy Policy(New)",
          link: "",
          active: false
        },
        {
          testo: "Ad choices",
          link: "",
          active: false
        },
        {
          testo: "Advertising",
          link: "",
          active: false
        },
        {
          testo: "Jobs",
          link: "",
          active: false
        },
        {
          testo: "Subscriptions",
          link: "",
          active: false
        },
        {
          testo: "Talent Workshops",
          link: "",
          active: false
        },
        {
          testo: "CPSC Certificates",
          link: "",
          active: false
        },
        {
          testo: "Ratings",
          link: "",
          active: false
        },
        {
          testo: "Shop Help",
          link: "",
          active: false
        },
        {
          testo: "Contact Us",
          link: "",
          active: false
        },
      ],
      sites: [
        {
          testo: "DC",
          link: "",
          active: false
        },
        {
          testo: "MAD Magazine",
          link: "",
          active: false
        },
        {
          testo: "DC Kids",
          link: "",
          active: false
        },
        {
          testo: "DC Universe",
          link: "",
          active: false
        },
        {
          testo: "DC Power Visa",
          link: "",
          active: false
        },
      ],
    };
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
    .fm-left{
      display: flex;
      flex-wrap: nowrap;
      align-items: flex-start;
      padding-top: 30px;
      div{
        width: calc(100% / 3);
      }
      ul{
        list-style-type: none;
        li{
          padding: 3px 0;
          color: $color-footer-mid-options;
        }
      }
      h4{
        margin: 10px 0;
        font-size: 1.5rem;
        color: white;
        text-transform: uppercase;
      }
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
