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
                    </li>
                </ul>
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
        height: 100px;

        #sezione {
            width: 60%;
            margin: auto;  
            
            #top-head {
                display: flex;
                justify-content: space-between;
                align-items: center;
                #nav-bar {
                    ul {
                        li {
                            display: inline;
                            margin: 0 20px;
                        }
                    }
                }

            }

        }

    }
</style>
