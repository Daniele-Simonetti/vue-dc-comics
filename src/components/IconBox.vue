<template>
  <div class="endmain">
    <li>
      <img :src="img" :alt="text">
      <a href="">{{text}}</a>
    </li>
  </div>
</template>

<script>
export default {
  name: "IconBox",
  props: {
    img: String,
    text: String
  }
}
</script>

<style lang="scss" scoped>
div.endmain {
  width: calc(100% / 5);
  li {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: center;
    // width: calc(100% / 5);
    a {
      display: block;
      text-decoration: none;
      padding: 1em;
      text-transform: uppercase;
      color: white;
    }
    img {
      width: 20%;
    }
    img.powershell {
      width: 28%;
    }
    img.maps {
      width: 15%;
    }
  }

}
</style>