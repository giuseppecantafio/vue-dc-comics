<template>
  <div>
    <main>
        <div class="main-wrapper">
            <h1>--&gt; Content goes here &lt;--</h1>
        </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "AppMain",
  data() {
    return {
      
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
main{
    margin-top: 3px;
    height: 150px;
    background-color: $bg-main;
    width: 100%;

    .main-wrapper{
        width: 80%;
        margin: 0 auto;
    }
    h1{
        height: 100%;
        line-height: 150px;
        vertical-align: middle;
        color: $light-color;
    }
}
</style>
