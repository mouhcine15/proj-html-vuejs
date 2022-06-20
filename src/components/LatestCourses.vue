<template>
  <div class="section">
<!-- titoli -->
    <h4 class="grey text-center">BEGIN YOUR JOURNEY AT MAXCOACH</h4>
    <div class="font-size-45 margin-top-20 text-center">Latest <p class="disp-inline green">Online Courses</p></div>
<!-- sezione corsi -->
    <div class="just-start wrap">
<!-- card dei corsi -->
        <div id="card" class="margin-top-50 width-360 radius-5" v-for="(item, i) in corsi" :key="i">
            <div>
                <img class="width-100-perc" :src="item.img" alt="">
            </div>
            <div class="pad-left-20">
                <div class="green font-size-20 pad-top-10">
                    <strong>{{item.price}}</strong>
                </div>
                <div class="font-size-20 pad-top-10">
                    <strong>{{item.overview}}</strong>
                </div>
                <div class="just-start pad-top-30 pad-bot">
                    <div class="grey">
                        <font-awesome-icon icon="fa-regular fa-file-lines" /> {{item.lessons}}
                    </div>
                    <div class="grey pad-left-20">
                        <font-awesome-icon icon="fa-regular fa-user" /> {{item.students}}
                    </div>
                </div>
            </div>
        </div>
    </div>
<!-- bottone -->
    <div class="just-center margin-top-50">
        <div id="bottone">
            <strong>View all courses <font-awesome-icon icon="fa-solid fa-arrow-right-long" /></strong>
        </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'LatestCourses',
    data () {
      return {
          corsi: [
            {
                img: require("../assets/motivation-course-06-480x298.jpg"),
                price: '$30.00',
                overview:'How to be Successful: Create A Growth Mindset For Success',
                lessons: '3 Lessons',
                students: '50 Students',
            },
            {
                img: require("../assets/motivation-course-05-480x298.jpg"),
                price: '$30.00',
                overview:'How to Build Confidence in Your Abilities',
                lessons: '3 Lessons',
                students: '50 Students',
            },
            {
                img: require("../assets/motivation-course-04-480x298.jpg"),
                price: '$20.00',
                overview:'Productivity Machine - Focus in a Distracted World',
                lessons: '5 Lessons',
                students: '50 Students',
            },
            {
                img: require("../assets/motivation-course-03-480x298.jpg"),
                price: '$20.00',
                overview:'Effective Time Management Mastery - Complete Guide',
                lessons: '18 Lessons',
                students: '50 Students',
            },
            {
                img: require("../assets/motivation-course-02-480x298.jpg"),
                price: '$25.99',
                overview:'Body Language Secrets for Entrepreneurs',
                lessons: '18 Lessons',
                students: '50 Students',
            },
            {
                img: require("../assets/motivation-course-01-480x298.jpg"),
                price: '$30.00',
                overview:'Management Skills: The science of Leadership',
                lessons: '17 Lessons',
                students: '50 Students',
            },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #card {
        margin:30px 10px;
    }
    #card:hover {
        box-shadow: 0px 0px 15px 15px rgb(237, 236, 236);
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
    .margin-top-50 {
        margin-top: 50px;
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
    .just-center {
        display: flex;
        justify-content: center;
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