<template>
  <div class="jumbotron ">
    <div class="container ">
      <div class="text-jumbo d-flex flex-column justify-content-center pt-5">    
          <h1 class="pt-5">Drive With Avada</h1>
          <h3>We offer the finest Driving tuition money can buy</h3>  
      </div>
    </div>

    <div class="offert-up">
      <div>
      
      <p>Demos</p>
      </div>
      <div>
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
      span{
        color: $primary-color;
        font-size: 10px;
        text-align:center;
        span{
          font-size: 20px;
          font-weight: 900;
        }
      }
      p{
        font-size: 12px;
        text-align: center;
      }
      
    }
  }
}

</style>