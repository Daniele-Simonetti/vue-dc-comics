<template>
  <div class="footer">
    <div class="container">
      <div class="left-col">
        <div class="DcComics">
          <h2>Dc comics</h2>
          <ul>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
          </ul>
          <h2>Shop</h2>
          <ul>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
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
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
          </ul>
        </div>
        <div class="Sites">
          <h2>Sites</h2>
          <ul>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
            </li>
            <li>
              <a href="">lorem</a>
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
        font-size: 1.4em;
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