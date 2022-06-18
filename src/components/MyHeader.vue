<template>
  <div id="header">
    <!-- barra dele icone laterali del jumbo -->
    <div id="bar-lat">
        <div class="icon">
            <font-awesome-icon icon="fa-solid fa-ruler"/>
        </div>
        <div class="icon">
            <font-awesome-icon icon="fa-solid fa-life-ring" />
        </div>
        <div class="icon">
            <font-awesome-icon icon="fa-solid fa-book" />
        </div>
        <div class="icon">
            <font-awesome-icon icon="fa-solid fa-cart-shopping" />
        </div>
    </div>
    <div id="sezione">
        <!-- parte alta del header con logi e navbar  -->
        <div id="top-head">
            <div id="logo">
                <img src="../assets/dark-logo.png" alt="">
            </div>
            <div id="nav-bar">
                <ul>
                    <li v-for="(item, i) in navbar" :key="i">
                        {{item}}
                        <font-awesome-icon icon="fa-solid fa-angle-down" />
                    </li>
                </ul>
            </div>
            <div class="social">
                <div class="icona">
                    <font-awesome-icon icon="fa-brands fa-twitter" />
                </div>
                <div class="icona">
                    <font-awesome-icon icon="fa-brands fa-facebook-f" /> 
                </div>
                <div class="icona">
                    <font-awesome-icon icon="fa-brands fa-instagram" />                  
                </div>
                <div class="icona">
                    <font-awesome-icon icon="fa-brands fa-linkedin" />
                </div>
            </div>
        </div>
        <!-- jumbotron -->
        <div class="jumbo">
            <!-- testo laterale -->
            <div class="text-p">
                <h3>
                    I'M WINGMAN
                </h3>
                <h1>
                    Peace On Earth A Wonderful Wish But No Way
                </h1>
                <div>
                    Success isn't overnight. It's when everyday you get a little better than day before. It all adds up.
                </div>
                <div id="bottone">
                    <strong>Get Started For Free <font-awesome-icon icon="fa-solid fa-arrow-right-long" /></strong>
                </div>
            </div>
            <!-- immagini in absolute  -->
            <div class="foto-p">
                <img id="img-tipo" src="../assets/home-movation-hero-image.png" alt="">
                <img id="fiori" src="../assets/home-movation-shape-face-600x534.png" alt="">
            </div>
        </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
  data () {
      return {
          navbar: ["Home", "Pages", "Courses","Features", "Blog", "Shop"]
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #header {
        background-image: url(../assets/background-pattern-wavify.png);
        position: relative;

        #bar-lat {
            display: flex;
            flex-direction: column;
            justify-content: flex-start;
            background-color: rgb(234, 233, 233);
            position: absolute;
            right: 0;
            top: 250px;
            border-bottom-left-radius: 10px;
            border-top-left-radius:  10px;

            .icon {
                padding: 10px;
            }
        }

        #sezione {
            width: 60%;
            margin: auto;  
            
            #top-head {
                display: flex;
                justify-content: space-between;
                align-items: center;
                color: rgba(107,103,136,255);
                padding-top: 30px;
                #logo {
                    img{
                        width: 200px;
                    }
                }
                #nav-bar {
                    ul {
                        li {
                            display: inline;
                            margin: 0 20px;
                        }
                    }
                }
                .social {
                    .icona {
                        margin: 0 10px;
                        display: inline;
                    }

                }

            }
            .jumbo {
                margin-top: 150px;
                display: flex;
                justify-content: flex-start;
                
                .text-p {
                    width: 450px;
                    padding-bottom: 200px;
                    h1 {
                        font-size: 50px;
                        padding: 20px 0;
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
                        margin-top: 30px;
                    }
                    #bottone:hover {
                        background-color: rgba(63,58,100,255);
                    }
                }
                .foto-p {
                    #img-tipo {
                        position: absolute;
                        bottom: 0;
                        right: 400px;
                        z-index: 10;
                    }
                    #fiori {
                       position: absolute;
                        bottom: 0;
                        right: 300px; 
                    }
                }
            }

        }

    }
</style>
