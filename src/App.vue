<template>
  <div id="app">
    <div class="row">
      <card id="card">
        <div class="wrapper">
          <img alt="drawers" id="drawers" src="./assets/drawers.jpg">
          <Test titre="Shift the overall look and feel by adding these wonderful touches to furniture in your home"/>
          <Test para1="Ever been in a room and felt like something was missing? Perhaps it felt slightly bare and uninviting. I’ve got some simple tips to help you make any room feel complete."/>
          <div class="author">
            <img src="./assets/avatar-michelle.jpg" alt="avatar-michelle">
            <div class="infos">
            <Test nom="Michelle Appleton"/>
            <Test date="28 Jun 2020"/>
            <Test fb="./assets/facebook-square-brands.svg"/>
            <Test twitter="./assets/twitter-square-brands.svg"/>
            <Test facebook="./assets/pintrest-brands.svg"/>  

            </div>
            <div id="app">
              <!-- <p v-show="isNinja">Invisible like a ninja!</p> -->
              <div>
                <ul v-show="!isNinja">
                  <li><img src="./assets/facebook-square-brands.svg" alt="facebook"></li>
                  <li><img src="./assets/twitter-brands.svg" alt="twitter"></li>
                  <li><img src="./assets/pinterest-brands.svg" alt="pinterest"></li>
                </ul>
              </div>
              <button v-on:click="isNinja = !isNinja"><img src="./assets/share-solid.svg" alt="share"></button>
            </div>
          </div>

        </div>
      </card>
    </div>

  </div>
</template>

<script>
  import Test from './components/Test.vue'
  export default {
    name: 'App',
    components:{
      Test
    },
    data() {
      return {
        // para1: "Ever been in a room and felt like something was missing? Perhaps it felt slightly bare and uninviting. I’ve got some simple tips to help you make any room feel complete.",
        // nom: "Michelle Appleton",
        // date: "28 Jun 2020",
        isNinja: true
      }

    },

  }
</script>

<style>
  #app {
    font-size: 13px;

    @font-face {
      font-family: "Manrope";
      src: local("Manrope"),
        url(./fonts/Manrope/static/Manrope-Medium.ttf) format("truetype");
    }
  }

  #title {
    font-size: 38px;
    font-family: Manrope;
    margin-left: 30%;
  }

  #drawers {
    height: 40%;
    border-radius: 5%;
    float: left;
  }

  img {
    height: 9vh;
    border-radius: 50%;
  }

  #nom {
    font-weight: bold;
    margin-left: 25%;
  }
  #date {
    margin-left: 30%;
  }

  #infos {
    margin-top: 30%;
  }
  #card {
    display: flex;
    max-width: 900px;
    margin: 50px auto 0;
  }

  .wrapper {
    background-color: white;
    position: relative;
    overflow: hidden;
    box-shadow: 0 19px 38px rgba(black, 0.3), 0 15px 12px rgba(black, 0.2);
  }

  .author {
    margin-left: 30%;
  }

  #para1 {
    margin-left: 30%;
  }
</style>