<template>
    <div class="section">
        <div class="width-60-perc margin-auto pad-top-bot-50">
            <div class="white just-between">
<!-- sezione di address  -->
                <div class="width-50-perc">
                    <h3>Address</h3>
                    <ul class="list-style-none pad-top-20 grey">
                        <li class="pad-top-10" v-for="(item, i) in address" :key="i">
                            {{item}}
                        </li>
                    </ul>
<!-- icone social -->
                    <div class="pad-top-10 grey">
                        <font-awesome-icon icon="fa-brands fa-facebook-square" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-twitter" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-instagram" class="icone"/>
                        <font-awesome-icon icon="fa-brands fa-linkedin" class="icone"/>
                    </div>
                </div>
<!-- sezione di destra -->
                <div class="just-around width-50-perc">
<!-- Explore-->
                    <div>
                        <h3>Explore</h3>
                        <ul class="list-style-none pad-top-20 grey">
                            <li class="pad-top-10" v-for="(item, i) in explore" :key="i">
                                {{item}}
                            </li>
                        </ul>
                    </div>
<!-- About Us -->
                    <div>
                        <h3>About Us</h3>
                        <ul class="list-style-none pad-top-20 grey">
                            <li class="pad-top-10" v-for="(item, i) in about" :key="i">
                                {{item}}
                            </li>
                        </ul>
                    </div>
<!-- Information -->
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
<!-- copyright  -->
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

// COLORI 
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
    .pad-top-10 {
        padding-top: 10px;
    }
    .pad-top-20 {
        padding-top: 20px;
    }
    .pad-top-bot-50 {
        padding: 50px 0;
    }
// WIDTH 
    .width-50-perc {
        width: 50%;
    }
    .width-60-perc {
        width: 60%;
    }
// FLEX
    .just-between {
        display: flex;
        justify-content: space-between;
    }
    .just-around {
        display: flex;
        justify-content: space-around;
    }
// LIST STILE 
    .list-style-none {
        list-style-type: none;
    }
</style>