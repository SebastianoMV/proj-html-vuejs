<template>
  <main class="">
    <!-- BEHIND THE WEELS -->
    
    <div class="">
      <div class="debug container d-flex justify-content-between">
        <div class="text-behind debug">
          <h2>Get Behind The Wheel</h2>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt id placeat magnam accusamus architecto necessitatibus at inventore hic illum. Omnis dolores hic odit provident iste nihil nisi eos accusamus unde.</p>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla nobis qui quo! Ducimus, temporibus maxime. A nostrum minus in, blanditiis itaque eius repellendus quibusdam odit minima perferendis vitae eaque natus.</p>
        </div>
        <div class="smv-w-50 debug margin-top-less-20">
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
    <div class="courses">
      <div class="container d-flex">
        <div class="courses-news margin-top-less-20">

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

    <!-- % -->
    <div class="">
      <div class="debug container">
        <div class="row">
          <div class="col debug"></div>
          <div class="col debug"></div>
          <div class="col debug"></div>
        </div>
      </div>
    </div>

      <!-- INSTRUCTORS -->
    <div class="">
      <div class=" container d-flex debug justify-content-between align-items-center">
        <div class="debug d-flex">
          <h3>Your Instructors</h3>
          <div class="debug">
            sdfg
          </div>
          <div class="debug">

          </div>
        </div>
      </div>
      <div class="debug container">
        <div class="row">
          <div class="col debug"></div>
          <div class="col debug"></div>
          <div class="col debug"></div>
        </div>
      </div>
    </div>

    <!-- TESTIMONIALS -->
    <div class="debug">
      <div class="debug container text-center">
        TESTIMONIALS
      </div>
    </div>

    <!-- BANNER NEWS -->
    <div class="debug">
      <div class="debug container d-flex flex-column align-items-center margin-top-less-20">
        <div>
          testo
        </div>
        <div>
          freccia
        </div>
      </div>
    </div>

     <!-- NEWSLETTERS -->
    <div class="debug">
      <div class="debug container d-flex flex-column align-items-center" >
        <h3>Sing up to our Newsletters</h3>
        <input type="text">
        <button>SUBSCRIBE</button>
      </div>
    </div>
  </main>
</template>

<script>
export default { 
  name: 'MainComp'
}
</script>

<style lang="scss" scoped>

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
    background-position: bottom left;
    background-size: cover;

    .courses-news{
      width: 40%;
      background-color: white;
      border-radius: 5px;
      margin-bottom: 30px;
    }

  }
}

</style>