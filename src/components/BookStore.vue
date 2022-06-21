<template>
<div>
    <div class="section just-between">
<!-- parte di sinistra con la lista -->
      <div class="width-40-perc">
          <h4 class="grey">BOOK STORE ONLINE</h4>
          <div class="font-size-45 margin-top-30">Be Alpha With <p class="green disp-inline">Wingman's Book</p></div>
<!-- lista -->
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
<!-- bottone  -->
          <div id="bottone">
              <strong>Get Free Ebook</strong>
          </div>
      </div>
<!-- parte di destra con i libri -->
      <div class="just-between">
<!-- libri  -->
          <div class="pad-right-20 text-center relative" v-for="(item, i) in books" :key="i">
            <div class="card">
                <img class="width-300" :src="item.img" alt="">
                <div class="margin-top-20">
                    <strong>{{item.title}}</strong>
                </div>
                <div class="green font-size-20 margin-top-20">
                    <strong>{{item.price}}</strong>
                </div>
            </div>
<!-- icone che devono comparire -->
            <div class="icone-card">
                <font-awesome-icon icon="fa-solid fa-magnifying-glass" class="icona" />
                <font-awesome-icon icon="fa-solid fa-cart-shopping" class="icona"/>
                <font-awesome-icon icon="fa-regular fa-heart" class="icona"/>
                <font-awesome-icon icon="fa-solid fa-signal" class="icona"/>
            </div>
          </div>
      </div>
    </div>
<!-- sezione con le aziende partner -->
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
    .card {
        z-index: 2;
        position: relative;
    }
    .card:hover {
        z-index: 0;
    }
    .icone-card {
        position: absolute;
        top: 60px;
        right: 20px;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
    }
    .icone-card:hover {
        z-index: 2;
    }
    .icone-card .icona {
        background-color: white;
        border-radius: 50%;
        padding: 10px;
        margin: 5px;
    }
    .icona:hover {
        transform: scale(1.2);
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
    .pad-right-20 {
        padding-left: 20px;
    }
// WIDTH 
    .width-300 {
        width: 300px;
    }
    .width-40-perc {
        width: 40%;
    }

// FONT 
    .font-size-20 {
        font-size: 20px;
    }
    .font-size-45 {
        font-size: 45px;
    }
// FLEX
    .just-between {
        display: flex;
        justify-content: space-between;
    }
    .just-center {
        display: flex;
        justify-content: center;
    }
    .align-center {
        display: flex;
        align-items: center;
    }
// DISPLAY
    .disp-inline {
        display: inline;
    }
// POSITION 
    .relative {
        position: relative;
    }
</style>