<template>
    <div class="section">
        <div class="width-60-perc margin-auto pad-top-bot-50">
            <div class="white just-between">
                <div class="width-50-perc">
                    <h3>Address</h3>
                    <ul class="list-style-none pad-top-20 grey">
                        <li class="pad-top-10" v-for="(item, i) in address" :key="i">
                            {{item}}
                        </li>
                    </ul>
                    <div class="pad-top-10 grey">
                        <font-awesome-icon icon="fa-brands fa-facebook-square" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-twitter" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-instagram" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-linkedin" class="icone"/>
                    </div>
                </div>
                <div class="just-around width-50-perc">
                    <div>
                        <h3>Explore</h3>
                        <ul class="list-style-none pad-top-20 grey">
                            <li class="pad-top-10" v-for="(item, i) in explore" :key="i">
                                {{item}}
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>About Us</h3>
                        <ul class="list-style-none pad-top-20 grey">
                            <li class="pad-top-10" v-for="(item, i) in about" :key="i">
                                {{item}}
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>Information</h3>
                        <ul class="list-style-none pad-top-20 grey">
                            <li class="pad-top-10" v-for="(item, i) in information" :key="i">
                                {{item}}
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="grey text-center pad-top-bot-50">
                <font-awesome-icon icon="fa-regular fa-copyright" /> 2020 Maxcoach. All Rights Reserved
            </div>
        </div>
    </div>
</template>

<script>

export default {
  name: 'RealStories',
    data () {
      return {
            address: [
                '382 NE 191st St # 87394 Miami, FL 33179-3899',
                '+1(305)547-9909(9am-5pm EST, Monday-Friday)',
                'Support@maxcoach.com'
            ],
            explore: [
                'Start here',
                'Blog',
                'About us'
            ],
            about: [
                'Success story',
                'Courses',
                'Contact Us'
            ],
            information: [
                'Membership',
                'Purchase guide',
                'Privacy policy',
                'Terms of service'
            ],
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .icone {
        font-size: 25px;
        padding-right: 30px;
    }
   .section {
        width: 100%;
        margin-top: 100px;
        background-color: black;
    }
    
// TEXT ALIGN 
    .text-center {
        text-align: center;
    }
// TEXT DECORATION 
    .underline {
        text-decoration: underline;
    }

// COLORI 
   .green {
        color: rgb(32,173,150);
   }
   .grey {
        color: grey;
   }
   .white {
    color: white;
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
    .pad-top-20 {
        padding-top: 20px;
    }
    .pad-top-bot-50 {
        padding: 50px 0;
    }
    .pad-bot {
        padding-bottom: 30px;
    }
// WIDTH 
    .width-80 {
        width: 80px;
    }
    .width-200 {
        width: 260px;
    }
    .width-50-perc {
        width: 50%;
    }
    .width-60-perc {
        width: 60%;
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
    }
// BORDER RADIUS
    .radius-5 {
        border-radius: 5px;
    }
    .radius-50-perc {
        border-radius: 50%;
    }
// LIST STILE 
    .list-style-none {
        list-style-type: none;
    }
</style>