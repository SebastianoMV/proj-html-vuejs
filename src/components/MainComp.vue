<template>
  <main class="">
    <!-- BEHIND THE WEELS -->
    
    <div class="">
      <div class="container d-flex justify-content-between">
        <div class="text-behind my-5">
          <h2>Get Behind The Wheel</h2>
          <p class="mt-5">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt id placeat magnam accusamus architecto necessitatibus at inventore hic illum. Omnis dolores hic odit provident iste nihil nisi eos accusamus unde.</p>
          <p class="my-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla nobis qui quo! Ducimus, temporibus maxime. A nostrum minus in, blanditiis itaque eius repellendus quibusdam odit minima perferendis vitae eaque natus.</p>
        </div>
        <div class="smv-w-50 margin-top-less-20 box-white-standard">
          first-lesson
        </div>
      </div>
    </div>

    <!-- BANNER START -->
    <div class="banner-start">
      <div class="container d-flex justify-content-between align-items-center py-5">
        <div>
          <h2>Start Learning to Drive Today</h2>
          <p>Give Us a call to schedule your first drive lesson</p>
        </div>
        
        <p>1-880-555-555</p>
      </div>
    </div>

    <!-- COURSES -->
    <div class="courses background-cover">
      <div class="container d-flex">
        <div class="courses-news margin-top-less-20 box-white-standard">

        </div>
        <div class="container-fluid debug">
          <div class="row">
            <div class="col debug"></div>
            <div class="col debug"></div>
            <div class="col debug"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- rate -->
    <div class="rate-bg">
      <div class="debug container">
        <div class="row">
          <div class="col debug box-white-standard border-top-green mx-1"></div>
          <div class="col debug box-white-standard border-top-green mx-1"></div>
          <div class="col debug box-white-standard border-top-green mx-1"></div>
        </div>
      </div>
    </div>

      <!-- INSTRUCTORS -->
    <div class="">
      <div class=" container  debug">
        <div class="debug d-flex">
          
          <div class="debug">
            <h3>Your Instructors</h3>
            sdfg
          </div>
          <div class="debug">
           <BtnComp btnString="more about us"/>
          </div>
        </div>
      </div>
      <div class="debug container">
        <div class="row">
          <div class="col debug border-top-green mx-1 box-white-standard"></div>
          <div class="col debug border-top-green mx-1 box-white-standard"></div>
          <div class="col debug border-top-green mx-1 box-white-standard"></div>
        </div>
      </div>
    </div>

    <!-- TESTIMONIALS -->
    <div class="debug testimonials-bg background-cover">
      <div class=" container text-center">
        TESTIMONIALS
      </div>
    </div>

    <!-- BANNER NEWS -->
    <div class="debug banner-news-bg background-cover">
      <div class=" container d-flex flex-column align-items-center margin-top-less-20 ">
        <div class="news-container text-center box-white-standard">
          <h3>Latest News</h3>
          <div></div>
          <BtnComp btnString="more from the blog"/>
        </div>
          <img src="../assets/img/latestnews-bottom.png" alt="">
      </div>
    </div>

     <!-- NEWSLETTERS -->
    <div class="newsletter-bg background-cover">
      <div class="debug container d-flex flex-column align-items-center" >
        <h3>Sing up to our Newsletters</h3>
        <input type="text">
        <button>SUBSCRIBE</button>
      </div>
    </div>
  </main>
</template>

<script>
import BtnComp from './BtnComp.vue';
export default {
    name: "MainComp",
    components: { BtnComp }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/utilities';

main{
  height: 100%;
  .text-behind{
    width: 45%;
  }


  //banner start
  .banner-start{
    background-image: url(../assets/img/horizontal-cta-background.jpg);
    background-position: center;
    background-size: cover;
    color: white;
  }

  //COURSES
  .courses{
    background-image: url(../assets/img/promise-background.jpg);
    background-position: center;
    background-size: cover;

    .courses-news{
      width: 40%;
      background-color: white;
      border-radius: 5px;
      margin-bottom: 30px;
    }

  }

  //rate
  .rate-bg{
    background-image: url(../assets/img/latestnews-bottom.png);
    background-size: contain;
    background-repeat: no-repeat;
    background-color: blue;
  }

  // testimonials
  .testimonials-bg{
    background-image: url(../assets/img/testimonial-background.jpg);
    height: 400px; //rimuovere
  }

  // banner news
  .banner-news-bg{
    background-image: url(../assets/img/latestnews-background.jpg);
    height: 400px; //rimuovere
    .news-container{
      width: 50%;
      height: 100%;
      background-color: white;
      border-radius: 3px;
      border-top: 3px solid #7094a9;
    }
    img{
      width: 50%;
    }
  }

  // newsletter
  .newsletter-bg{
    background-image: url(../assets/img/newsletter_background.jpg);
  }
}

</style>