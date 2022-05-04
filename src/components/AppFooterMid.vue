<template>
  <div>
      <div class="footer-mid">
          <div class="footer-mid-wrapper debug">
              <div class="fm-left debug">
                  <ul>
                      <li v-for="(item, index) in navElm" :key="index">{{item.name}}</li>
                  </ul>
              </div>
              <div class="fm-right debug">
                  
              </div>
          </div>
      </div>
  </div>
</template>

<script>
import {data} from "./components/AppHeader.vue";

export default {
  name: "AppFooterMid",
  components: {
      data
  },
  data() {
    return {
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
@import "../style/generals";
.footer-mid{
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;
    width: 100%;

    .footer-mid-wrapper{
        width: 80%;
        height: 100%;
        margin: 0 auto;
        display: flex;

        .fm-left,
        .fm-right{
            width: 50%;
            height: 100%;
        }
        .fm-right{
            background-image: url("../assets/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }
    }
}
</style>
