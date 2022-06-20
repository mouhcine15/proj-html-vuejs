<template>
<div>
    <div id="main">
      <!-- statistiche e prestazioni -->
      <div id="stats">
          <div class="card" v-for="(item, i) in stats" :key="i">
              <div id="num-stat">
                  <strong>{{item.stat}}</strong>
              </div>
              <div id="name-stat">
                  <strong>{{item.names}}</strong>
              </div>
          </div>
      </div>
      <!-- sezione di AboutMe - presentazione -->
      <AboutMe/>
      <!-- sezione di Latest Online Courses - corsi -->
      <LatestCourses/>
      <!-- sezone del Book store -->
      <BookStore/>
    </div>
      <!-- sezione del Carousel -->
      <RealStories/>
</div>

</template>

<script>
import AboutMe from './AboutMe.vue';
import LatestCourses from './LatestCourses.vue';
import BookStore from './BookStore.vue';
import RealStories from './RealStories.vue';
export default {
    name: "MyMain",
    components: {
    AboutMe,
    LatestCourses,
    BookStore,
    RealStories
},
    data () {
      return {
          stats: [
            {
                stat: '1.926',
                names: 'FINISHED LESSONS',
            },
            {
                stat: '100%',
                names: 'SATISFACTION RATE',
            },
            {
                stat: '3092+',
                names: 'ENROLLED RATE',
            },
            {
                stat: '200',
                names: 'ONLINE INSTRUCTIONS',
            },
            ]
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   #main {
    width: 60%;
    margin: auto;
    margin-top: 100px;

        #stats {
            display: flex;
            justify-content: center;
            .card {
                padding: 0 60px;
                display: flex;
                flex-direction: column;
                align-items: center;
                border-right: 1px dashed  rgba(32,173,150,255);
                #num-stat {
                    color: rgba(32,173,150,255);
                    font-size: 50px;
                }
                #name-stat {
                    margin-top: 20px;
                }
            }
            .card:first-child {
                border-left: 1px dashed rgba(32,173,150,255);
            }
        }
   }
</style>