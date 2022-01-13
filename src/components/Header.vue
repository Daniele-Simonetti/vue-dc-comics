<template>
<div class="header">
  <div class="container">
    <img src="../assets/img/dc-logo.png" alt="logo header">
    <ul>
      <li>
        <a href="">Characters</a>
      </li>
      <li>
        <a href="">Comics</a>
      </li>
      <li>
        <a href="">Movies</a>
      </li>
      <li>
        <a href="">Tv</a>
      </li>
      <li>
        <a href="">Games</a>
      </li>
      <li>
        <a href="">Collectibles</a>
      </li>
      <li>
        <a href="">Videos</a>
      </li>
      <li>
        <a href="">Fans</a>
      </li>
      <li>
        <a href="">News</a>
      </li>
      <li>
        <a href="">Shop</a>
      </li>
    </ul>
  </div>

</div>
</template>

<script>
export default {
  name: "Header",
  data() {},
};
</script>

<style lang="scss" scoped>
  @import "../assets/scss/partials/_variables.scss";
  .header {
    // background-color: red;
    img {
      width: 7%;
      padding: 1em 0;
    }
  }
  .container {
    display: flex;
    justify-content: space-around;
  }
  ul {
    width: 100%;
    list-style: none;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    li {
      height: 100%;
      display: flex;
      align-items: center;
      a {
        display: block;
        text-decoration: none;
        padding: 1em;
        font-weight: bold;
        text-transform: uppercase;
        color: $headerGrayColor;
      }
    }
  }
</style>