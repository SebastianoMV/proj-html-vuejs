<template>
  <div class="jumbotron ">
    <div class="container ">
      <div class="text-jumbo d-flex flex-column justify-content-center pt-5">    
          <h1 class="pt-5">Drive With Avada</h1>
          <h3>We offer the finest Driving tuition money can buy</h3>  
      </div>
    </div>

    <div class="offert-up">
      <div class="d-flex flex-column justify-content-center align-items-center">
      <img src="../assets/img/download.png" alt="">
      <p>Demos</p>
      </div>
      <div class="d-flex flex-column justify-content-center align-items-center">
        <span>$ <span>39</span> </span>
        <p>On Sale</p>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'JumboComp'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/var';

.jumbotron{
  background-image: url(../assets/img/homepage-hero-background.jpg);
  background-position: center;
  background-size: cover;
  height: 600px;
  position: relative;
  .container{
    height: 100%;
    .text-jumbo{
      color: white;
      width: 50%;
      height: 100%;
      h1{
        font-size: 3rem;
      }
    }
  }
  .offert-up{
    position: fixed;
    z-index: 999;
    top: 110px;
    right: 10px;
    div{
      height: 50px;
      width: 50px;
      background-color: white;
      border-radius: 10px;
      margin: 5px;
      img{
        width: 20px;
      }
      span{
        color: $primary-color;
        font-size: 10px;
        
        span{
          font-size: 20px;
          font-weight: 900;
        }
      }
      p{
        font-size: 12px;
        margin: auto;
      }
      
    }
  }
}

</style>