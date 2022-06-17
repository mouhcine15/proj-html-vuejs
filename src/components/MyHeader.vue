<template>
  <div id="header">
    <div id="sezione">
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
        <div class="jumbo">
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
            <div id="foto-p">
                <img src="../assets/home-movation-hero-image.png" alt="">
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
        height: 700px;

        #sezione {
            width: 60%;
            margin: auto;  
            
            #top-head {
                display: flex;
                justify-content: space-between;
                align-items: center;
                color: rgba(107,103,136,255);
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
                padding-top: 150px;
                display: flex;
                justify-content: flex-start;
                
                .text-p {
                    width: 450px;
                }
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
                #foto-p {
                    
                }
            }

        }

    }
</style>
