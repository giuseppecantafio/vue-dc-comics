<template>
  <div>
    <div class="jumbotron">
      <span class="button">Current series</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
@import "../style/generals";

.jumbotron {
  margin-top: 3px;
  background-image: url("../assets/img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
  width: 100%;
  position: relative;

  .button {
    @include jb-main-buttons;
    height: 50px;
    font-size: 1.5rem;
    position: absolute;
    bottom: -25px;
    left: 155px;
  }
}
</style>
