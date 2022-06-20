<template>
<div>
    <div class="section just-between">
      <div class="width-40-perc">
          <h4 class="grey">BOOK STORE ONLINE</h4>
          <div class="font-size-45 margin-top-30">Be Alpha With <p class="green disp-inline">Wingman's Book</p></div>
          <div>
              <ul id="list" class="margin-top-30">
                  <li class="margin-top-20">
                      <font-awesome-icon icon="fa-solid fa-check" class="green"/>
                      <span class="grey">
                          Help you understand yourself better
                      </span>
                  </li>
                  <li class="margin-top-20">
                      <font-awesome-icon icon="fa-solid fa-check" class="green"/>
                      <span class="grey">
                          Revealing mature tips
                      </span>
                  </li>
                  <li class="margin-top-20">
                      <font-awesome-icon icon="fa-solid fa-check" class="green"/>
                      <span class="grey">
                          Give right advice
                      </span>
                  </li>
                  <li class="margin-top-20">
                      <font-awesome-icon icon="fa-solid fa-check" class="green"/>
                      <span class="grey">
                          Fascinating examples of alpha man
                      </span>
                  </li>
              </ul>
          </div>
          <div id="bottone">
              <strong>Get Free Ebook</strong>
          </div>
      </div>
      <div class="just-between">
          <div class="pad-right-20 text-center relative card" v-for="(item, i) in books" :key="i">
              <img class="width-300" :src="item.img" alt="">
              <div class="margin-top-20">
                  <strong>{{item.title}}</strong>
              </div>
              <div class="green font-size-20 margin-top-20">
                  <strong>{{item.price}}</strong>
              </div>
              <div class="icone-card">
                  <font-awesome-icon icon="fa-solid fa-magnifying-glass" class="icona" />
                  <font-awesome-icon icon="fa-solid fa-cart-shopping" class="icona"/>
                  <font-awesome-icon icon="fa-regular fa-heart" class="icona"/>
                  <font-awesome-icon icon="fa-solid fa-signal" class="icona"/>
              </div>
          </div>
      </div>
    </div>
    <div class="section align-center just-center">
        <img src="../assets/client-logo-05-primary.png" alt="">
        <img src="../assets/client-logo-06-primary.png" alt="">
        <img src="../assets/client-logo-07-primary.png" alt="">
        <img src="../assets/client-logo-04-primary.png" alt="">
        <img src="../assets/client-logo-03-primary.png" alt="">
        <img src="../assets/client-logo-02-primary.png" alt="">
    </div>

</div>
</template>

<script>

export default {
  name: 'BookStore',
    data () {
      return {
          books: [
            {
                img: require("../assets/product-book-11-400x400.jpg"),
                title:'Alpha man by Maxcoach',
                price: '$29.00'
            },
            {
                img: require("../assets/product-book-10-400x400.jpg"),
                title:'Alpha man by Maxcoach',
                price: '$39.00',
            }
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #list li {
        list-style-type: none;
    }
    #bottone {
        background-color: rgba(32,173,150,255);
        color: white;
        width: 250px;
        height: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 5px;
        margin-top: 40px;
    }
    #bottone:hover {
        background-color: rgba(63,58,100,255);
    }
    .icone-card {
        position: absolute;
        top: 60px;
        right: 20px;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
    }
    .icone-card .icona {
        background-color: white;
        border-radius: 50%;
        padding: 10px;
        margin: 5px;
    }

    .align-center img {
        padding: 40px;
        filter: grayscale(0.7);
    }
    
   .section {
        width: 100%;
        margin-top: 100px;
    }

// TEXT ALIGN 
    .text-center {
        text-align: center;
    }
// COLORI 
   .green {
        color: rgb(32,173,150);
   }
   .grey {
        color: grey;
   }

// MARGINI-PADDING
    .margin-top-20 {
        margin-top: 20px;
    }
    .margin-top-30 {
        margin-top: 30px;
    }
    .margin-top-50 {
        margin-top: 50px;
    }
    .margin-top-100 {
        margin-top: 100px;
    }
    .padding-50 {
        padding: 50px;
    }
    .pad-right-20 {
        padding-left: 20px;
    }
    .pad-top-10 {
        padding-top: 10px;
    }
    .pad-top-30 {
        padding-top: 30px;
    }
    .pad-bot {
        padding-bottom: 30px;
    }
// WIDTH 
    .width-200 {
        width: 200px;
    }
    .width-300 {
        width: 300px;
    }
    .width-40-perc {
        width: 40%;
    }
    .width-50-perc {
        width: 50%;
    }
    .width-100-perc {
        width: 100%;
    }

// FONT 
    .font-size-20 {
        font-size: 20px;
    }
    .font-size-45 {
        font-size: 45px;
    }
// FLEX
    .just-start {
        display: flex;
        justify-content: flex-start;
    }
    .just-between {
        display: flex;
        justify-content: space-between;
    }
    .just-center {
        display: flex;
        justify-content: center;
    }
    .just-around {
        display: flex;
        justify-content: space-around;
    }
    .align-center {
        display: flex;
        align-items: center;
    }
    .wrap {
        display: flex;
        flex-wrap: wrap;
    }
    .flex-verticale {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
    }
// DISPLAY
    .disp-inline {
        display: inline;
    }
    .disp-none {
        display: none;
    }
// POSITION 
    .relative {
        position: relative;
    }
    .absolute {
        position: absolute;
        top: 70px;
        right: 10px
    }
// BORDER RADIUS
    .radius-5 {
        border-radius: 5px;
    }
</style>