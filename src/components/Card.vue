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
  span {
    display: block;
    color: white;
    text-transform: uppercase;
    font-size: 1.1em;
    margin: 1em 0;
  }
</style>