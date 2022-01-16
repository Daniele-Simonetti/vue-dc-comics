<template>
<div class="header">
  <div class="container">
    <img src="../assets/img/dc-logo.png" alt="logo header">
    <ul>
      <li v-for="(link, index) in links" :key="index" @click="activeLink(index)">
        <a :href="link.url" :class="(link.current == true) ? 'active' : '' ">{{link.title}}</a>
      </li>
      <!-- <li>
        <a href="" class="active">Comics</a>
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
      </li> -->
    </ul>
  </div>

</div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          title: "Characters",
          url: "#",
          current: false,
        },
        {
          title: "Comics",
          url: "#",
          current: true,
        },
        {
          title: "Movies",
          url: "#",
          current: false,
        },
        {
          title: "Tv",
          url: "#",
          current: false,
        },
        {
          title: "Games",
          url: "#",
          current: false,
        },
        {
          title: "Collectibles",
          url: "#",
          current: false,
        },
        {
          title: "Videos",
          url: "#",
          current: false,
        },
        {
          title: "Fans",
          url: "#",
          current: false,
        },
        {
          title: "News",
          url: "#",
          current: false,
        },
        {
          title: "Shop",
          url: "#",
          current: false,
        },
      ]
    }
  },
  methods: {
    activeLink(indexLink) {
      this.links.forEach(
        (link, index) => {
          if (index === indexLink) {
            link.current = true;
          } else {
            link.current = false;
          }
        }
      )
    }
  }
};
</script>

<style lang="scss" scoped>
  @import "../assets/scss/partials/_variables.scss";
    img {
      width: 7%;
      padding: 1em 0;
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
          display: flex;
          align-items: center;
          text-decoration: none;
          padding: 0 1em;
          font-weight: bold;
          text-transform: uppercase;
          color: $headerGrayColor;
          height: 100%;
          &:hover,
          &:active,
          &.active {
            border-bottom: 5px solid $mainBlueColor;
          }
        }
      }
    }
  .container {
    display: flex;
  }
</style>