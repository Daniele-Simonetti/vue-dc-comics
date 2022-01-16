<template>
  <div class="footer">
    <div class="container">
      <div class="left-col">
        <div class="DcComics">
          <h2>Dc comics</h2>
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
              <a href="">TV</a>
            </li>
            <li>
              <a href="">Games</a>
            </li>
            <li>
              <a href="">Videos</a>
            </li>
            <li>
              <a href="">News</a>
            </li>
          </ul>
          <h2>Shop</h2>
          <ul>
            <li>
              <a href="">Shop DC</a>
            </li>
            <li>
              <a href="">SHop DC Collectibles</a>
            </li>
          </ul>
        </div>
        <div class="Dc">
          <h2>Dc</h2>
          <ul>
            <li>
              <a href="">Terms Of Use</a>
            </li>
            <li>
              <a href="">Privacy policy (New)</a>
            </li>
            <li>
              <a href="">Ad Choices</a>
            </li>
            <li>
              <a href="">Advertising</a>
            </li>
            <li>
              <a href="">Jobs</a>
            </li>
            <li>
              <a href="">Subscriptions</a>
            </li>
            <li>
              <a href="">Talent Workshops</a>
            </li>
            <li>
              <a href="">CPSC Certificates</a>
            </li>
            <li>
              <a href="">Ratings</a>
            </li>
            <li>
              <a href="">Shop Help</a>
            </li>
            <li>
              <a href="">Contact us</a>
            </li>
          </ul>
        </div>
        <div class="Sites">
          <h2>Sites</h2>
          <ul>
            <li>
              <a href="">DC</a>
            </li>
            <li>
              <a href="">Mad Magazine</a>
            </li>
            <li>
              <a href="">DC Kids</a>
            </li>
            <li>
              <a href="">DC Universe</a>
            </li>
            <li>
              <a href="">DC Power Visa</a>
            </li>
          </ul>
        </div>
        <!-- <div class="Shop">
          <h2>Shop</h2>
          <ul>
            <li>lorem</li>
            <li>lorem</li>
          </ul>
        </div> -->
      </div>
      <div class="right-col">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {

  },
}
</script>

<style lang="scss" scoped>
  @import "../assets/scss/partials/_variables.scss";
  .container {
    display: flex;
  }
  .footer {
    background-image: url(../assets/img/footer-bg.jpg);
    
  }
  .left-col {
    width: 40%;
    margin-bottom: 4em;
    display: flex;
    // flex-wrap: wrap;
    div {
      width: calc(100% / 3);
      height: 100%;
      h2 {
        color: white;
        text-transform: uppercase;
        padding-top: 1em;
        padding-bottom: 0.5em;
      }
    }
    li {
      list-style: none;
      a {
        text-decoration: none;
        color: $footerGrayColor;
        font-size: 1em;
      }
    }
  
  }
  .right-col {
    width: calc(100% - 40%);
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: auto;
    background-position: right;
    
  }
</style>