<template>
  <footer>
    <!-- FOOTER -->
    <div class="footer-bg background-cover">
      <div class="container">
        <div class="row py-5">
          <div class="col">
            <img src="../assets/img/avada-drivers-logo-2x-400x77.png" alt="">
            <p>Avada Driving School is the right choisefor experiencedrivers looking for a refresher course, or  the brand new driver waiting to pass firt time</p>
          </div>
          <div class="col">
            <h4>Contact details</h4>
            <ul>
              <li>12345 North Main Street, New York, NY 55555</li>
              <li>1.800.555.6789</li>
              <li>info@your-domain.com</li>
              <li>Theme-Fusion.com</li>
            </ul>
          </div>
          <div class="col courses-li">
            <h4>Courses</h4>
            <ul>
              <li>Pass Plus</li>
              <li>Intensive Course</li>
              <li>Automatic</li>
              <li>Instructor Training</li>
            </ul>
          </div>
          <div class="col text-center">
            <img src="../assets/img/footer-ad-grid.png" alt="">
            <BtnComp btnString="book nows"/>
          </div>
        </div>
      </div>
    </div>

     <!-- BANNER COPY -->
    <div class="copy-bg background-cover">
      <div class="container py-4 d-flex justify-content-between align-items-center">
      <p>&copy;Copiright 2022 | Avada Theme by <span>SMV</span> | All Rights Reserved | Powered by <span>SICURAMENTE NON WORDPRESS</span></p>
      <div>
        <i class="fa-brands fa-facebook-f mx-2"></i>
        <i class="fa-brands fa-twitter mx-2"></i>
        <i class="fa-brands fa-youtube mx-2"></i>
        <i class="fa-brands fa-instagram mx-2"></i>
        
      </div>
    </div>
    </div>
  </footer>
  
</template>

<script>
import BtnComp from './BtnComp.vue';


export default {
    name: "FooterComp",
    components: { BtnComp }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/utilities';
  .footer-bg{
    background-image: url(../assets/img/footer-background-color.jpg);
    color: gray;
    font-size: 13px;
  }
  h4{
    color: white;
    text-transform: uppercase;
  }
  img{
    width: 90%;
    margin-bottom: 20px;
  }
  .courses-li{
      li{
        color: $primary-color;
        font-size: 15px;
      }
    }


  .copy-bg{
    background-color: black;
    color: grey;
    font-size: 10px;
    span{
      color: $primary-color;
    }
    i{
      color: white;
      font-size: 15px;
    }
    
  }

</style>