<template>
  <div>
    <div class="jumbotron"></div>
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
.jumbotron{
  margin-top: 3px;
  background-image: url("../assets/img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
  width: 100%;

}
</style>
