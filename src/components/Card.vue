<template>
  <div class="card">
    <div>
    <img :src="img" :alt="name">
    </div>
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
  width: calc(192px - 2em);
  margin: 1em 1em;
  div {
    overflow: hidden;
    width: 100%;
    height: 160px;
    img {
      width: 100%; 
    }
  }
  span {
    display: block;
    color: white;
    text-transform: uppercase;
    font-size: 1.1em;
    margin-top: 0.5em;
  }
}
</style>