<template>
  <div class="section">
<!-- scritta ABOT ME iniziale -->
    <div class="green-color">
        <h3>ABOUT ME</h3>
    </div>
<!-- sezione di testo -->
    <div class="margin-top-50 just-between">
<!-- grande tirolo -->
        <div class="width-40-perc font-size-45">
            How to Be an Alpha Male: The 15 Habits of True Alphas
        </div>
<!-- parte sinistra di testo  -->
        <div class="width-55-perc">
            <h3><strong>Want tolearn hoe to be <p class="green-color disp-inline">an alpha male</p>? How to be more masculine? How to be the man you've always wanted to be?</strong></h3>
            <div class="margin-top-30">
                Your goal is to show the consistency of business, core values, and customer care. Puctuality, responsability, individuality, accurcy, enthusiasm - you have to clearly explain how these qualities are applicable to your work. And the important thing is you do love what you do.
            </div>
        </div>
    </div>
    <div class="margin-top-100 just-start align-center">
<!-- immagine con player YouTube -->
            <div>
                <img src="../assets/home-movation-video-poster-670x450.jpg" alt="">
            </div>
            <div class="padding-50">
                <h2>
                    "Every morning you have two choises: continue to sleep with your dreams, or wake up and chase them."
                </h2>
                <div class="margin-top-50">
                    <img class="margin-top-20" src="../assets/home-movation-shape-01.png" alt="">
                    <h3 class="margin-top-20">
                        Kaixa Stark
                    </h3>
                    <div class="margin-top-20">
                        WINGMAN
                    </div>
                </div>

            </div>
        </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   .section {
    width: 100%;
    margin-top: 100px;
    }


// COLORI 
   .green-color {
    color: rgb(32,173,150);
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
// WIDTH 
    .width-40-perc {
        width: 40%;
    }
    .width-55-perc {
        width: 55%;
    }

// FONT 
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
    .align-center {
        display: flex;
        align-items: center;
    }
// DISPLAY
    .disp-inline {
        display: flex;
        display: inline;
    }
</style>