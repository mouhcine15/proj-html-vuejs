<template>
    <div class="section just-start relative">
        <div id="left-side" class="text-center">
            <h2 class="green margin-top-100">REAL STORIES</h2>
            <div class="margin-top-70">
                <h2 class="width-50-perc margin-auto">
                    {{slides[attivazione].text}}
                </h2>
                <img class="radius-50-perc width-80 margin-top-30" :src="slides[attivazione].img"  alt=""/>
                <h3 class="margin-top-20">
                    {{slides[attivazione].name}}
                </h3>
                <div class="grey margin-top-20">
                    {{slides[attivazione].profession}}
                </div>
            </div>
        </div>
        <div class="controller">
            <div class="grey">
                <font-awesome-icon icon="fa-solid fa-caret-up" />
            </div>
            <div>
                1/4
            </div>
            <div @click="previusslide()" class="grey">
                <font-awesome-icon icon="fa-solid fa-sort-down" />
            </div>
        </div>
        <div id="right-side" @click="nextslide()">
            
        </div>
    </div>
</template>

<script>

export default {
  name: 'RealStories',
    data () {
        return {
            slides: [
                {
                    text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
                    img: require('../assets/testimonial-avata-02.jpg'),
                    name: 'Mina Hollace',
                    profession: '/ FreeLancer'
                },
                {
                    text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
                    img: require('../assets/testimonial-avata-02.jpg'),
                    name: 'Mina Hollace',
                    profession: '/ FreeLancer'
                },
                {
                    text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
                    img: require('../assets/testimonial-avata-02.jpg'),
                    name: 'Mina Hollace',
                    profession: '/ FreeLancer'
                },
                {
                    text: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.',
                    img: require('../assets/testimonial-avata-02.jpg'),
                    name: 'Mina Hollace',
                    profession: '/ FreeLancer'
                },
            ],
            attivazione: 0,
        }
    },
    methods: {
        nextslide(){
            this.attivazione ++;
            if (this.attivazione >= this.slides.length-1) {
                this.attivazione = 0;
            }
        },
        
        previusslide(){
            this.attivazione --;
            if (this.attivazione < 0) {
                this.attivazione = this.slides.length-1;
            }
        },
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   .section {
        width: 100%;
        margin-top: 100px;
    }
    #left-side {
        background-image: linear-gradient(rgba(170, 170, 170, 0.1), rgba(170, 170, 170, 0.1)), url(../assets/background-pattern-wavify.png);
        height: 701px;
        width: 50%;
    }
    #right-side {
        background-image: url(../assets/home-movation-testimonial-image-768x562.jpg);
        width: 50%;
        background-repeat: no-repeat;
        background-size: contain;
    }
    .controller {
        position: absolute;
        top: 300px;
        right: 905px;
        background-color: rgb(255, 255, 255);
        border-radius: 50%;
        padding: 20px 35px;
        display: flex;
        flex-direction: column;
        align-items: center;
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
   .white-back {
    background-color: rgb(195, 27, 27);
   }

// MARGINI-PADDING
    .margin-auto {
        margin: auto;
    }
    .margin-top-20 {
        margin-top: 20px;
    }
    .margin-top-30 {
        margin-top: 30px;
    }
    .margin-top-70 {
        margin-top: 70px;
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
    .width-80 {
        width: 80px;
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
        right: 950px
    }
// BORDER RADIUS
    .radius-5 {
        border-radius: 5px;
    }
    .radius-50-perc {
        border-radius: 50%;
    }
</style>