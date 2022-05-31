<template>
  <main class="">

    <!-- BEHIND THE WEELS -->
    <div class="behind-weels">
      <div class="container d-flex justify-content-between">
        <div class="text-behind my-5">
          <h2>Get Behind The Wheel</h2>
          <p class="mt-5 top-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt id placeat magnam accusamus architecto necessitatibus at inventore hic illum.</p>
          <p class="my-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla nobis qui quo! Ducimus, temporibus maxime. A nostrum minus in, blanditiis itaque eius repellendus quibusdam odit minima perferendis vitae eaque natus.</p>
        </div>
        <div v-if="form"  class="smv-w-50 margin-top-less-20 box-white-standard d-flex flex-column justify-content-between text-center p-5">
          <h3>First Lesson Free!</h3>
          <p>When you make a block booking with us your first lesson is included for free.</p>
          <input type="text" placeholder="Your Name*">
          <input type="email" placeholder="Email*">
          <input type="text" placeholder="Telephone">
          <input type="text" placeholder="Location">
          <div @click="showForm()">
            <BtnComp btnString="request a callback"/>
          </div>
          
        </div>
        <div @click="showForm()" v-else class="m-auto"> 
          <BtnComp btnString="request a callback"/>
        </div>
      </div>
    </div>

    <!-- BANNER START -->
    <div class="banner-start">
      <div class="container d-flex justify-content-between align-items-center py-5">
        <div>
          <h2>Start Learning to Drive Today</h2>
          <h6>Give Us a call to schedule your first drive lesson</h6>
        </div>
        
        <p><i class="fa-solid fa-phone-flip"></i> 1-880-555-555</p>
      </div>
    </div>

    <!-- COURSES -->
    <div class="courses background-cover">
      <div class="container d-flex justify-content-between">
        <div class="courses-news margin-top-less-20 box-white-standard">
          <img src="../assets/img/new-corner.jpg" alt="new corner">
          <div class="text-center px-5 mb-5">
            <h3>Courses</h3>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Inventore doloremque nam modi facilis, incidunt necessitatibus reprehenderit facere  earum autem provident nobis at optio praesentium itaque commodi laborum neque quo similique!</p>
            <BtnComp btnString="course information"/>
          </div>
        </div>
        <div class="courses-cards container-fluid">
          <div class="row">
            <div class="col">
              <div class="card-course text-center my-5">
                <img src="../assets/img/courses-passplus.jpg" alt="courses-passplus">
                <h4>Pass Plus</h4>
                <BtnComp2 btnString="learn more" />
              </div>
            </div>
            <div class="col">
              <div class="card-course text-center my-5">
                <img src="../assets/img/course-intensive.jpg" alt="courses-intensive">
                <h4>Intensive</h4>
                <BtnComp2 btnString="learn more" />
              </div>
            </div>
            <div class="col">
              <div class="card-course text-center my-5">
                <img src="../assets/img/courses-instructor.jpg" alt="courses-instructor">
                <h4>Instructor</h4>
                <BtnComp2 btnString="learn more" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- RATE -->
    <div class="rate-bg">
      <div class="container">
        <div class="row">
          <div class="col box-white-standard border-top-green mx-1">
            <RateComp ratePercent="95"/>
            <h5>pass rate</h5>
          </div>
          <div class="col box-white-standard border-top-green mx-1">
            <RateComp ratePercent="100"/>
            <h5>referral rate</h5>
          </div>
          <div class="col box-white-standard border-top-green mx-1">
            <RateComp ratePercent="0"/>
            <h5>accident rate</h5>
          </div>
        </div>
      </div>
    </div>

      <!-- INSTRUCTORS -->
    <div class="instructors">
      <div class=" container ">
        <div class="d-flex justify-content-between align-items-center my-5">
          
          <div class="text-instructors">
            <h3>Your Instructors</h3>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam id facere dolorem tempora in, a quia mollitia, voluptatibus possimus dolore officiis. Quis beatae, tempore veniam sunt consectetur non voluptatem iste.</p>
          </div>
          <div class="">
           <BtnComp btnString="more about us"/>
          </div>
        </div>
      </div>
      <div class="container margin-bot-less-20">
        
          <InstructorsCardComp />

      </div>
    </div>

    <!-- TESTIMONIALS -->
    <div class="testimonials-bg background-cover p-5">
      <div class=" container-testimonials m-auto text-center py-4">
        <h3 class="my-3">Testimonials</h3>
        <p>Here's what our happy drivers had to say sbout our service</p>
        <CarouselComp/>
      </div>
    </div>

    <!-- BANNER NEWS -->
    <div class="banner-news-bg background-cover">
      <div class=" container d-flex">
        <div class=" d-flex flex-column align-items-center margin-top-less-20">
          <div class="news-container text-center box-white-standard ">
            <h3 class="my-5">Latest News</h3>
            <div class="container-fluid">
              <div class="row my-5">
                <div class="col">
                  <div>
                    <img src="../assets/img/blog-choosecar-700x441.jpg" alt="blog choosecar">
                    <h5>What Car to Start With?</h5>
                    <p>February 7th 2019 | <span>0 comments</span></p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                  </div>
                </div>
                <div class="col">
                  <div>
                    <img src="../assets/img/blogpost-10and2-700x441.jpg" alt="blog post">
                    <h5>Avada Driving School Expanding</h5>
                    <p>February 7th 2019 | <span>0 comments</span></p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                  </div>
                </div>
              </div>
            </div>
            <BtnComp btnString="more from the blog"/>
          </div>
          <img src="../assets/img/latestnews-bottom.png" alt="">
        </div>
      </div>
    </div>

     <!-- NEWSLETTERS -->
    <div class="newsletter-bg background-cover">
      <div class="container d-flex flex-column align-items-center py-4" >
        <h3 class="py-4">Sing up to our Newsletters</h3>
        <input type="text">
        <BtnComp btnString="subscribe" class="py-3 width-btn"/>
        <p>(we do not share your data with anybody, and only use it for its intended porpose)</p>
      </div>
    </div>
  </main>
</template>

<script>
import BtnComp from './BtnComp.vue';
import RateComp from './RateComp.vue';
import CarouselComp from './CarouselComp.vue';
import BtnComp2 from './BtnComp2.vue';
import InstructorsCardComp from './InstructorsCardComp.vue';
export default {
    name: "MainComp",
    components: { BtnComp, RateComp, CarouselComp, BtnComp2, InstructorsCardComp },
    data() {
      return {
        form: false,
      }
    },
    methods: {
      showForm(){
        this.form = !this.form;
        console.log(this.form);
      }
    },
}
</script>

<style lang="scss" scoped>
@import '../assets/style/utilities';

main{
  height: 100%;
  .text-behind{
    width: 45%;
  }

  //behind
  .behind-weels{
    margin-bottom: 40px;
    h3{
      color: $primary-color;
    }
    .top-text{
      font-size: 20px;
    }
    p{
      color: #8d959f;
    }
    input{
      padding: 12px;
      margin-bottom: 25px;
      background-color: #f7f7f7;
      border: 1px solid lightgray;
      border-radius: 5px;
      color: #7094a9;
    }
  }

   //banner start
  .banner-start{
    background-image: url(../assets/img/horizontal-cta-background.jpg);
    background-position: center;
    background-size: cover;
    color: white;
    p{
      font-size: 25px;
    }
  }

  //COURSES
  .courses{
    background-image: url(../assets/img/promise-background.jpg);
    background-position: center;
    background-size: cover;
    .courses-news{
      // position: absolute;
      width: 35%;
      background-color: white;
      border-radius: 10px;
      margin-bottom: 30px;
      overflow: hidden;
      img{
        // position: relative;
        // top: 0;
        // left: 0;
        width: 60px;
      }
    }
    .courses-cards{
      width: 60%;
      img{
        width: 90%;
      }
    }
  }

  //RATE
  .rate-bg{
    background-image: url(../assets/img/output-onlinepngtools.png);
    background-size: contain;
    background-repeat: no-repeat;
    background-position-y: top;
    h5{
      color: #8d959f;
      text-align: center;
      text-transform: uppercase;
      margin-top: 30px;
      margin-bottom: 40px;
    }
    
    
  }

  //INSTRUCTORS
  .instructors{
    color: #8d959f;
    .text-instructors{
    width: 80%;
    color: black;
    }
    h4{
      color: black;
    }
    img{
      width: 100%;
    }
    .col:hover{
      transform: scale(1, 1.05);
    }
  }
  

  // TESTIMONIALS
  .testimonials-bg{
    background-image: url(../assets/img/testimonial-background.jpg);
    .container-testimonials{
      width: 40%; 
    }
  }

  // banner news
  .banner-news-bg{
    background-image: url(../assets/img/latestnews-background.jpg);
    padding-bottom: 40px;
    .news-container{
      width: 100%;
      height: 100%;
      background-color: white;
      border-top-right-radius: 5px;
      border-top-left-radius: 5px;
      border-bottom-right-radius: 0px;
      border-bottom-left-radius: 0px;
      border-top: 4px solid #7094a9;
      p{
        color: gray;
      }
      h5 , span {
        color: $primary-color;
      }
      h5{
        margin-top: 20px;
      }
    }
    img{
      width: 100%;
    }
  }

  // newsletter
  .newsletter-bg{
    background-image: url(../assets/img/newsletter_background.jpg);
    .container{
      width: 30%;
      margin: auto;
      input{
        width: 100%;
      }
    
    }
  }
}

</style>