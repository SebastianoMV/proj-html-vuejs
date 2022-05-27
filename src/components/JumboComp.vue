<template>
  <div class="debug">
    <div class="container ">
      <div class="text-jumbo debug d-flex flex-column justify-content-center pt-5">
        
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

div{
  height: 400px;
  position: relative;
  .container{
    height: 100%;
    .text-jumbo{
      width: 50%;
    }
  }
  .offert-up{
    position: absolute;
    top: 100px;
    right: 10px;
    div{
      height: 50px;
      width: 50px;
      background-color: white;
      z-index: 999;
      border-radius: 10px;
      margin: 5px;
    }
  }
}

</style>