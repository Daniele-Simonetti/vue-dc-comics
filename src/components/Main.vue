<template>
  <div class="main">
    <div class="jumbo">
      <div class="currentser">
        <span>Current series</span>
      </div>
    </div>
    <div class="container">
      <div class="cards">
        <Card 
        v-for="(card, index) in cards" 
        :key="index"
        :img="card.thumb"
        :name="card.series"
        />
        <!-- <div class="card" v-for="(card, index) in cards" :key="index">
          <img :src="card.thumb" :alt="card.type">
        </div> -->
      </div>
      <div class="load-more">
        <button>Load More</button>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "./Card.vue" 
export default {
  name: "Main",
  components: {
    Card,
  },
  data() {
    return {
      cards: 
        [
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
            "price": "$19.99",
            "series": "Action Comics",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
            "price": "$3.99",
            "series": "American Vampire 1976",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
            "price": "$16.99",
            "series": "Aquaman",
            "type": "graphic novel"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
            "price": "$2.99",
            "series": "Batgirl",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            "price": "$3.99",
            "series": "Batman",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            "price": "$2.99",
            "series": "Batman Beyond",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
            "price": "$3.99",
            "series": "Batman/Superman",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
            "price": "$4.99",
            "series": "Batman/Superman Annual",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
            "price": "$5.99",
            "series": "Batman: The Joker War Zone",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
            "price": "$6.99",
            "series": "Batman: Three Jokers",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
            "price": "$4.99",
            "series": "Batman: White Knight Presents: Harley Quinn",
            "type": "comic book"
          },
          {
            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
            "price": "$16.99",
            "series": "Catwoman",
            "type": "graphic novel"
          }
        ]
    }
  },
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
  .main {
    background-color: $cardbgColor;
  }
  h2 {
    color: white;
    padding: 1.5em 0;
  }
  .jumbo {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 265px;
    background-repeat: no-repeat;
    background-size: cover;
    div.currentser {
      position: relative;
      span {
        text-transform: uppercase;
        font-weight: bold;
        font-size: 1.2em;
        color: white;
        background-color: $mainBlueColor;
        padding: 0.3em 1.2em;
        position: absolute;
        top: 245px;
        left: 208px;
      }
    }
  }
  div.cards {
    display: flex;
    flex-wrap: wrap;
    padding-top: 3em;
  }
  div.load-more {
    text-align: center;
    button {
      background-color: $wardBlueColor;
      border: 0;
      color: white;
      text-transform: uppercase;
      font-weight: bold;
      padding: 0.8em 3.5em;
      margin-bottom: 1.5em;
    }
  }
</style>