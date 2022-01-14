<template>
  <div class="card">
    <img :src="img" :alt="name">
    <span>{{ name }}</span>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    img: String,
    name: String
  }
}
</script>

<style lang="scss" scoped>
.card {
  width: calc((100% / 6) - 2em);
  height: calc((100% / 6) - 2em);
  margin: 0 1em;
  img {
    object-fit: cover;
  }
  span {
    display: block;
    color: white;
    text-transform: uppercase;
    font-size: 1.1em;
    margin: 0.5em 0 2em 0;
  }
}
</style>