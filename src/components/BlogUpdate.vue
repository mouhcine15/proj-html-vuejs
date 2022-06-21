<template>
    <div class="section">
        <div>
            <h4 class="grey">BLOG UPDATED</h4>
          <div class="font-size-45 margin-top-30">Interesting<p class="green disp-inline"> articles updated</p> daily</div>
        </div>
<!-- sezione delle card  -->
        <div class="just-between margin-top-50">
<!-- card  -->
            <div class="width-200 card" v-for="(item, i) in articles" :key="i">
                <img class="width-100-perc radius-5" :src="item.img" alt="">
                <div>
                    <div class="grey margin-top-20">
                        <font-awesome-icon icon="fa-regular fa-calendar" />  {{item.date}}
                    </div>
                    <h3 class="margin-top-20">
                        {{item.title}}
                    </h3>
                    <div class="grey margin-top-20">
                        {{item.overview}}
                    </div>
                </div>
            </div>
        </div>
<!-- link View More -->
        <div class="green underline text-center margin-top-50 bigger-1-1">
            <h3>VIEW ALL POSTS</h3>
        </div>
    </div>
</template>

<script>

export default {
  name: 'RealStories',
    data () {
      return {
          articles: [
            {
                img: require("../assets/motivation-blog-04-480x325.jpg"),
                date: 'May 13,2020',
                title:'How to Stay True to Your Personal Brand',
                overview: 'When it comes to your business or career, ypu want...'
            },
            {
                img: require("../assets/motivation-blog-03-480x325.jpg"),
                date: 'May 13,2020',
                title:'5 Vital Lessons in 5 Years of Freelancing',
                overview: "Being self-employed and working from home, it's easy to get...",
            },
            {
                img: require("../assets/motivation-blog-02-480x325.jpg"),
                date: 'May 13,2020',
                title:'11 Super Useful Tips for Small-Business Owners',
                overview: 'Being a small-business owner poses a ton of challenges. We...'
            },
            {
                img: require("../assets/motivation-blog-01-480x325.jpg"),
                date: 'May 13,2020',
                title:'How to Give Yourself Grace to Start Again',
                overview: 'Forgive yourself for bad habits you may have started or...'
            },
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   .section {
        width: 100%;
        margin-top: 100px;
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
        color: rgb(93, 93, 93);
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
// WIDTH 
    .width-200 {
        width: 260px;
    }
    .width-100-perc {
        width: 100%;
    }

// FONT 
    .font-size-45 {
        font-size: 45px;
    }
// FLEX
    .just-between {
        display: flex;
        justify-content: space-between;
    }
// DISPLAY
    .disp-inline {
        display: inline;
    }
// BORDER RADIUS
    .radius-5 {
        border-radius: 5px;
    }
// BIGGER
    .bigger-1-1:hover {
        transform: scale(1.1);
    }
</style>