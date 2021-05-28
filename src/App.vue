<template>
  <div id="app">

    <section>

      <div  id="first-section">

        <img id="pizza1" alt="pizza" src="./assets/layer.png">

        <Menu></Menu>

        <hashtag class="hashtag"></hashtag>

        <ribbon></ribbon>

        <read-more class="read-more"></read-more>

        <MyLabel msg="GRAND" class="grand"></MyLabel>

        <MyLabel msg="OPENING" class="opening"></MyLabel>

      </div>

    </section>



    <section>

      <div id="second-section">

        <img alt="pizza.exe" src="./assets/RightPizza.png">

        <MyLabel class="what-new" msg="What new?"></MyLabel>

        <rectangle class="rectangle"></rectangle>

        <OfferMenu></OfferMenu>

        <MyLabel msg="new format" class="new-format"></MyLabel>

      </div>

    </section>

    <section>

      <div id="third-section">

        <guide class="guide"  msg="| new format" text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut malesuada vitae nisl eu pharetra."></guide>

        <guide class="guide"  msg="|| Master class" text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut malesuada vitae nisl eu pharetra."></guide>

        <guide class="guide"  msg="||| pizza restaurant" text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut malesuada vitae nisl eu pharetra."></guide>

      </div>

    </section>

    <section>

      <div id="fourth-section">

        <img alt="Pizza" src="./assets/Pizzabackground.png">

        <MyLabel msg="#pizzeria." class="pizza-hashtag"></MyLabel>

        <MyLabel msg="OUR NEW MENU" class="our-new-menu"></MyLabel>

        <yellow-back class="yellow-menu"></yellow-back>

        <dish-list class="dishes"></dish-list>

        <dishes-legend class="dishLegend" ></dishes-legend>

        <menu-price-back class="dishPricesBack"></menu-price-back>

        <dish-price class="dishPrice"></dish-price>

      </div>

    </section>

    <section>

      <div id="fifth-section">

        <my-label class="our-concept-title" msg="ABOUT OUR CONCEPT"></my-label>

        <my-label class="our-concept-text" msg="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec imperdiet lorem ut accumsan posuere. Vivamus ullamcorper metus purus, sit amet varius sem elementum nec."></my-label>

        <concept-links class="our-concept-links"></concept-links>

      </div>

    </section>

  </div>
</template>

<script>
  import hashtag from "@/components/Atoms/Labels/hashtag-box"
  import ribbon from "@/components/Atoms/Decorations/yellow-ribbon.vue"
  import readMore from "@/components/Atoms/Buttons/read-more.vue"
  import rectangle from "@/components/Atoms/Decorations/yellow-rectangle.vue"
  import OfferMenu from "@/components/Moleculs/Offer-menu.vue"
  import guide from "@/components/Moleculs/guide-menu.vue"
  import Menu from "@/components/Moleculs/Menu"
  import MyLabel from "@/components/Atoms/Labels/Mylabel.vue"
  import yellowBack from "@/components/Atoms/Decorations/yellow-menu-background.vue"
  import dishList from "@/components/Moleculs/Dishes-list.vue"
  import DishesLegend from "@/components/Moleculs/Dishes-legend"
  import menuPriceBack from "@/components/Atoms/Decorations/yellow-menu-prices.vue"
  import dishPrice from "@/components/Moleculs/Dishes-Prices.vue"
  import conceptLinks from "@/components/Moleculs/Concept-link.vue"


  export default {
    name: 'App',
    components: {

      hashtag, ribbon, readMore,  Menu, MyLabel,

      rectangle, OfferMenu,

      guide,

      yellowBack, dishList, DishesLegend, menuPriceBack, dishPrice,

      conceptLinks,

    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: -10px;
    align-items: stretch;
    display: -ms-flexbox;
  }

  #pizza1{
    padding: 0;
  }

  #first-section{
    position: relative;
    width: 1434px;
    height: 960px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding: 0;
    border: #FFBA00 2px solid;
  }

  #second-section {
    position: relative;
    width: 1434px;
    height: 610px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    border: #FFBA00 2px solid;
  }

  #second-section img {
    float: right;
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    margin: auto;
  }

  #third-section {
    width: 1434px;
    height: 375px;
    background-color: #FFBA00;
    margin-left: auto;
    margin-right: auto;
    border: #FFBA00 2px solid;
    position: relative;
  }

  #fourth-section {
    position: relative;
    width: 1434px;
    height: 1200px;
    margin-left: auto;
    margin-right: auto;
    border: #FFBA00 2px solid;
  }

  #fourth-section img {
    width: 1434px;
    height: 1200px;
    margin-left: auto;
    margin-right: auto;
  }

  #fifth-section {
    height: 410px;
    width: 1434px;
    margin-left: auto;
    margin-right: auto;
    border: #FFBA00 2px solid;
    position: relative;
  }

  .rectangle {
    position: absolute;
    top: 35%;
    left: 10%;
  }

  .hashtag {
    top: 30px;
    position: absolute;
  }

  .read-more {
    position: absolute;
    top: 57%;
    left: 57%;
  }

  .grand .texting {
    position: absolute;
    font-weight: bolder;
    font-size: 120px;
    font-family: 'Noto Sans JP', sans-serif;
    color: white;
    top: 43%;
    left: 14%;
    margin: 0;
  }

  .opening .texting {
    position: absolute;
    top: 44%;
    left: 14%;
    color: white;
    font-family: 'Assistant', sans-serif;
    font-size: 110px;
    letter-spacing: 13px;
  }

  .what-new .texting {
    position: absolute;
    text-align: center;
    top: 20%;
    left: 20%;
    color: white;
    font-size: 44px;
    letter-spacing: 10px;
    margin: 0;
    padding: 0;
  }



  .new-format .texting {
    position: absolute;
    transform: rotate(-90deg);
    top: 42%;
    left: 3%;
    font-family: 'Open Sans Condensed', sans-serif;
    color: white;
    font-size: 65px;
    font-weight: lighter;
    letter-spacing: 8px;
    padding: 0;
  }

  .guide {
    display: inline-block;
    padding: 0;
    margin-left: 25px;
    margin-right: 25px;
  }

  .pizza-hashtag .texting {
    position: absolute;
    display: flex;
    top: 5%;
    left: 43%;
    color: #FFBA00;
    font-size: 40px;
    font-family: 'Varela Round', sans-serif;
    font-weight: 600;
    letter-spacing: 3px;
  }

  .our-new-menu .texting {
    position: absolute;
    display: flex;
    color: #FFBA00;
    font-size: 80px;
    border: white 4px solid;
    top: 10%;
    left: 25%;
    padding: 10px 50px 50px 50px;
    font-family: 'Varela Round', sans-serif;
  }

  .yellow-menu {
    position: absolute;
    border: #FFBA00 4px solid;
    top: 35%;
    left: 27%;
  }

  .dishes {
    position: absolute;
    top: 38%;
    left: 30%;
  }

  .dishLegend {
    position: absolute;
    top: 89%;
    left: 28%;
  }

  .dishPricesBack {
    position: absolute;
    top: 38%;
    left: 90%;
  }

  .dishPrice {
    position: absolute;
    top: 38%;
    left: 90%;
  }

  .our-concept-title .texting {
    color: #FFBA00;
    font-family: 'Assistant', sans-serif;
    font-size: 40px;
    font-weight: 600;
    margin: 0;
    padding: 0;
    position: absolute;
    left: 38%;
    top: 20%;
  }

  .our-concept-text .texting {
    font-size: 20px;
    width: 850px;
    position: absolute;
    left: 22%;
    top: 35%;
  }

  .our-concept-links{
    position: absolute;
    left: 35%;
    top: 60%;
  }



  body {
    background-color: #242424;
  }
</style>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Assistant&display=swap');
</style>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:wght@300&display=swap');
</style>
