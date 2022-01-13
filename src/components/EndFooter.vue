<template>
  <div class="endfooter">
    <div class="container">
      <button>Sign-up now!</button>
      <ul>
        <li>
          <a href="">Follow Us</a>
        </li>
        <li>
          <img src="../assets/img/footer-facebook.png" alt="facebook">
        </li>
        <li>
          <img src="../assets/img/footer-twitter.png" alt="twitter">
        </li>
        <li>
          <img src="../assets/img/footer-youtube.png" alt="youtube">
        </li>
        <li>
          <img src="../assets/img/footer-pinterest.png" alt="pinterest">
        </li>
        <li>
          <img src="../assets/img/footer-periscope.png" alt="periscope">
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "EndFooter",
  data() {

  },
}
</script>

<style lang="scss" scoped>
  @import "../assets/scss/partials/_variables.scss";

  .endfooter {
    background-color: $endFooterColor;
    
    .container {
      display: flex;
      justify-content: space-between;
      padding: 1.5em 0;
      ul {
        list-style: none;
        display: flex;
        align-items: center;
        li {
          padding: 0 0.5em;
          a {
            width: 16%;
            text-decoration: none;
            color: $wardBlueColor;
            text-transform: uppercase;
            font-weight: bold;
          }
          img {
            width: 80%;
          }
        }
      }
      button {
        background-color: $endFooterColor;
        border: 2px solid $mainBlueColor;
        text-transform: uppercase;
        color: white;
        padding: 1em 1.5em;
      }
    }
  }
</style>