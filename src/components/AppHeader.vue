<template>
  <div>
    <header>
      <nav>
        <div class="img-container"><img src="../assets/img/dc-logo.png" alt="dc logo" /></div>
        <ul>
          <li
            v-for="(item, index) in navElm"
            :key="index"
            :class="{ selected: item.active }"
          >
            {{ item.name }}
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      navElm: [
        {
          name: "Character",
          link: "",
          active: false,
        },
        {
          name: "Comics",
          link: "",
          active: true,
        },
        {
          name: "Movies",
          link: "",
          active: false,
        },
        {
          name: "Tv",
          link: "",
          active: false,
        },
        {
          name: "Games",
          link: "",
          active: false,
        },
        {
          name: "Collectibles",
          link: "",
          active: false,
        },
        {
          name: "Videos",
          link: "",
          active: false,
        },
        {
          name: "Fans",
          link: "",
          active: false,
        },
        {
          name: "News",
          link: "",
          active: false,
        },
        {
          name: "Shop",
          link: "",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables";
header {
  background-color: $bg-header;
  height: 100px;
  width: 80%;
  margin: 0 auto;

  nav {
    display: flex;
    justify-content: center;
    gap: 200px;
  }
  .img-container{
    height: 80px;
    margin-top: 10px;
  }
  img{
    padding-right: 200px;
    height: 100%;
    width: 100%;
    object-fit: contain;
  }
  ul {
    list-style-type: none;
    line-height: 100px;
    vertical-align: middle;
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }
  li {
    display: inline-block;
  }
  .selected {
    color: $color-header-selected;
    border-bottom: 2px solid $color-header-selected;
  }
}
</style>
