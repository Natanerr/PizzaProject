<template>
  <div id="app">

    <img src="./assets/ScrollButton.png" alt="Scroll Button" class="top" id="top" @click="scrollToTop">

    <section>

      <div  id="first-section">

        <img id="pizza1" alt="pizza" src="./assets/layer.png">

        <Menu class="media-menu"></Menu>

        <hashtag class="hashtag"></hashtag>

        <yellow-ribbon></yellow-ribbon>

        <read-more class="read-more"></read-more>

        <MyLabel msg="GRAND" class="grand"></MyLabel>

        <MyLabel msg="OPENING" class="opening"></MyLabel>

      </div>

    </section>



    <section>

      <div id="second-section">

        <img class="image-pizza2" alt="pizza.exe" src="./assets/RightPizza.png">

        <MyLabel class="what-new" msg="What new?"></MyLabel>

        <rectangle class="rectangle"></rectangle>

        <OfferMenu></OfferMenu>

        <MyLabel msg="new format" class="new-format"></MyLabel>

      </div>

    </section>

    <div id="specialAnchor"></div>

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

    <section>

      <div id="sixth-section">

        <img alt="MasterClass" src="./assets/MasterClass.png">

        <yellow-master class="yellow-master"></yellow-master>

        <Apply class="Apply"></Apply>

        <my-label msg="MASTERCLASS" class="master-title"></my-label>

        <my-label class="MasterDescription" msg="| THE RECIPE FOR THE MOST DELICIOUS PIZZA DOUGH |"></my-label>

        <my-label class="MasterSlogan" msg="waiting for you!"></my-label>

        <my-label class="MasterPrice" msg="PRICE 15$"></my-label>

        <my-label class="MasterTime" msg="12:00-15:00"></my-label>

      </div>

    </section>

    <section>

      <div id="seventh-section">

        <my-label class="gallery-title" msg="GALLERY"></my-label>

        <img class="gallery-first" alt="Gallery-first" src="./assets/Gallery1stPicture.png">

        <img class="gallery-second" alt="Gallery-second" src="./assets/Gallery2Picture.png">

        <img class="gallery-third" alt="Gallery-third" src="./assets/Gallery3Picture.png">


      </div>

    </section>

    <footer>

      <div class="footer-wrapper" id="footer">

        <div class="float">
          <footer-component msg="About"></footer-component>
        </div>

        <grid-label1></grid-label1>

        <grid-label2></grid-label2>

        <grid-label3></grid-label3>

      </div>

    </footer>
  </div>
</template>

<script>
  import hashtag from "@/components/Atoms/Labels/hashtag-box";
  import readMore from "@/components/Atoms/Buttons/read-more.vue";
  import rectangle from "@/components/Atoms/Decorations/yellow-rectangle.vue";
  import OfferMenu from "@/components/Moleculs/Offer-menu.vue";
  import guide from "@/components/Moleculs/guide-menu.vue";
  import Menu from "@/components/Moleculs/Menu";
  import MyLabel from "@/components/Atoms/Labels/Mylabel.vue";
  import yellowBack from "@/components/Atoms/Decorations/yellow-menu-background.vue";
  import dishList from "@/components/Moleculs/Dishes-list.vue";
  import DishesLegend from "@/components/Moleculs/Dishes-legend";
  import menuPriceBack from "@/components/Atoms/Decorations/yellow-menu-prices.vue";
  import dishPrice from "@/components/Moleculs/Dishes-Prices.vue";
  import conceptLinks from "@/components/Moleculs/Concept-link.vue";
  import yellowMaster from "@/components/Atoms/Decorations/yellow-master-description.vue";
  import Apply from "@/components/Atoms/Buttons/Apply";
  import footerComponent from "@/components/Moleculs/footer-component.vue";
  import gridLabel1 from "@/components/Atoms/Labels/grid-label1.vue";
  import gridLabel2 from "@/components/Atoms/Labels/grid-label2.vue";
  import gridLabel3 from "@/components/Atoms/Labels/grid-label3.vue";
  import yellowRibbon from "@/components/Atoms/Decorations/yellow-ribbon";


  export default {
    name: 'App',
    components: {

      hashtag, readMore,  Menu, MyLabel, yellowRibbon,

      rectangle, OfferMenu,

      guide,

      yellowBack, dishList, DishesLegend, menuPriceBack, dishPrice,

      conceptLinks,

      yellowMaster, Apply,

      footerComponent, gridLabel1, gridLabel2, gridLabel3,

    },
    methods: {
        scrollToTop() {
          document.getElementById("top").onclick = function () {
            window.scrollTo(0,0);
          }
        }
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

  #sixth-section {
    width: 1434px;
    height: 1200px;
    border: #FFBA00 2px solid;
    margin-left: auto;
    margin-right: auto;
    position: relative;
  }

  #sixth-section img {
    width: 1434px;
    height: 1200px;
    margin-right: auto;
    margin-left: auto;
  }

  #seventh-section {
    width: 1434px;
    height: 930px;
    position: relative;
    margin-left: auto;
    margin-right: auto;
    border: #FFBA00 2px solid;
  }

  .top {
    position: fixed;
    right: 2%;
    bottom: 3%;
    width: 100px;
    height: auto;
  }

  .media-menu {
    position: absolute;
    top: 5%;
    right: 1%;
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
    top: 50%;
    left: 65%;
  }

  .grand .texting {
    position: absolute;
    font-weight: bolder;
    font-size: 130px;
    font-family: Alef, sans-serif;
    top: 39%;
    left: 8%;
    margin: 0;
    color: transparent;
    background: url(assets/back.png);
    -webkit-text-stroke: 2px #ffffff;
    -webkit-background-clip: text;
    animation: back 20s linear infinite;
  }

  @keyframes back {
    100% {
      background-position: 2000px 1000px;
    }
  }

  .opening .texting {
    position: absolute;
    top: 39%;
    left: 12%;
    color: transparent;
    background: url(assets/back.png);
    -webkit-text-stroke: 2px #ffffff;
    -webkit-background-clip: text;
    animation: back2 20s linear infinite;
    font-family: Alef, sans-serif;
    font-size: 130px;
    font-weight: bolder;
    letter-spacing: 13px;
  }

  @keyframes back2 {
    100% {
      background-position: 2000px 0;
    }
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

  .yellow-master {
    position: absolute;
    top: -10%;
    left: 645px;
    bottom: 0;
    right: 0;
  }

  .Apply {
    position: absolute;
    top: 80%;
    left: 836px;
    bottom: 0;
    right: 0;
  }

  .master-title .texting {
    position: absolute;
    top: 4%;
    left: 61%;
    font-size: 60px;
    font-weight: 600;
  }

  .MasterDescription .texting {
    position: absolute;
    width: 430px;
    top: 23%;
    left: 57%;
    font-size: 50px;
    text-align: left;
    font-weight: 600;
  }

  .MasterSlogan .texting {
    position: absolute;
    top: 47%;
    left: 57%;
    font-size: 45px;
    font-weight: 600;
    font-family: 'Assistant', sans-serif;
  }

  .MasterPrice .texting {
    position: absolute;
    top: 56%;
    left: 72%;
    font-weight: 600;
    font-size: 43px;
    font-family: 'Assistant', sans-serif;
  }

  .MasterTime .texting {
    position: absolute;
    top: 60%;
    left: 72%;
    font-weight: 600;
    font-size: 43px;
    font-family: 'Assistant', sans-serif;
  }

  .gallery-title .texting {
    font-size: 80px;
    font-weight: 700;
    color: #FFBA00;
    font-family: 'Assistant', sans-serif;
  }

  .gallery-first {
    float: left;
    top: 0;
    bottom: 0;
    right: 0;
    margin: auto;
  }

  .gallery-third {
    float: right;
    top: 0;
    bottom: 0;
    right: 0;
    margin: auto;
  }

  .footer-wrapper {
    border: orange 2px solid;
    border-bottom: none;
    border-top: none;
    width: 1434px;
    height: 320px;
    margin: 0 auto;
    background-color: #FFBA00;
  }

  @media (max-width:1437px ) {
    #app {
      max-width: 970px;
    }
  }

  @media (max-width:992px ) {
    #app {
      max-width: 750px;
    }
  }

  @media (max-width:767px ) {
    #app {
      max-width: none;
    }

    p { font-size: 20px}

    .new-format { display: none; }

    .grand .texting , .opening .texting {
      font-size: 150px;
      font-weight: bold;
      font-family: Alef, sans-serif;
    }

    .yellow-menu { display: none; }

    .dishPricesBack { display: none; }

    .grand .texting { left: 2%; top: 40%; }

    .opening .texting { left: 45%; top: 27%;}

    .media-menu {
      font-family: Alef, sans-serif;
      font-size: 70px;
      font-weight: bolder;
      right: 12%;
    }

    .what-new .texting  {
      left: 5%;
      font-weight: bolder;
    }

    .image-pizza2 {
      height: 100%;
      width: 100%;
    }

  }


  footer {
    width: 100%;
    height: 320px;
    background-color: #FFBA00;
  }

  body {
    background-color: #242424;
    margin:0;
  }
</style>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Assistant&display=swap');
</style>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:wght@300&display=swap');
</style>
