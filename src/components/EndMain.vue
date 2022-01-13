<template>
  <div class="Endmain">
    <div class="container">
      <ul class="endmain">
        <li>
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
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "EndMain",
  data() {

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
    padding: 3em 0;
  }
  li {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: center;
    width: calc(100% / 5);
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
</style>