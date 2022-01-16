<template>
  <div class="Endmain">
    <div class="container">
      <ul class="endmain">
        <IconBox 
        v-for="(icon, index) in iconbox"  :key="index"
        :img="icon.src"
        :text="icon.text"
        />
        <!-- <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
          <a href="">Digital comics</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="dc merch">
          <a href="">Dc merchandise</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="sbscription">
          <a href="">Subscription</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator" class="maps">
          <a href="">Comic shop locator</a>
        </li>
        <li>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power vis" class="powershell">
          <a href="">Dc power visa</a>
        </li> -->
      </ul>
    </div>
  </div>
</template>

<script>
import IconBox from "./IconBox.vue"
export default {
  name: "EndMain",
  components: {
    IconBox,
  },
  data() {
    return {
      iconbox: [
        {
          "src": require("../assets/img/buy-comics-digital-comics.png"),
          "text": "Digital comics"
        },
        {
          "src": require("../assets/img/buy-comics-merchandise.png"),
          "text": "Digital comics"
        },
        {
          "src": require("../assets/img/buy-comics-subscriptions.png"),
          "text": "Digital comics"
        },
        {
          "src": require("../assets/img/buy-comics-shop-locator.png"),
          "text": "Digital comics"
        },
        {
          "src": require("../assets/img/buy-dc-power-visa.svg"),
          "text": "Digital comics"
        },
      ]
    }
  },
}
</script>

<style lang="scss" scoped>
  @import "../assets/scss/partials/_variables.scss";
  .Endmain {
    background-color: $mainBlueColor;
    // height: 150px;
    z-index: 1;
  }
  ul.endmain {
    display: flex;
    justify-content: space-around;
    padding: 2em 0;
  }
  // li {
  //   list-style: none;
  //   display: flex;
  //   align-items: center;
  //   justify-content: center;
  //   width: calc(100% / 5);
  //   a {
  //     display: block;
  //     text-decoration: none;
  //     padding: 1em;
  //     text-transform: uppercase;
  //     color: white;
  //   }
  //   img {
  //     width: 20%;
  //   }
  //   img.powershell {
  //     width: 28%;
  //   }
  //   img.maps {
  //     width: 15%;
  //   }
  // }
</style>