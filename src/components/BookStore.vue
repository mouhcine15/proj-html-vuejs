<template>
  <div class="section">
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
  </div>
</template>

<script>

export default {
  name: 'BookStore',
    
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
    .pad-left-20 {
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
    .width-360 {
        width: 360px;
    }
    .width-40-perc {
        width: 40%;
    }
    .width-55-perc {
        width: 55%;
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
    .align-center {
        display: flex;
        align-items: center;
    }
    .wrap {
        display: flex;
        flex-wrap: wrap;
    }
// DISPLAY
    .disp-inline {
        display: inline;
    }
// BORDER RADIUS
    .radius-5 {
        border-radius: 5px;
    }
</style>