<template>
  <div class="jumbotron">
    <div class="container ">
      <div class="text-jumbo d-flex flex-column justify-content-center pt-5">
        
          <h1>Drive With Avada</h1>
          <h3>We offer the finest Driving tuition money can buy</h3>
        
      </div>
      
    </div>

    <div class="offert-up">
      <div>

      </div>
      <div>

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
    top: 100px;
    right: 10px;
    div{
      height: 50px;
      width: 50px;
      background-color: white;
      border-radius: 10px;
      margin: 5px;
      z-index: 999;
    }
  }
}

</style>