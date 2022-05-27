<template>
  <header>
      <div class="banner-top-nav">
        <div class="container d-flex justify-content-between py-2">
          <span>We have a 95% Successful Pass Rate!</span>
          <span>Give us a call</span>
        </div>
      </div>
      <nav>
        <div class="container d-flex ">
          <img src="" alt="">
          <ul class="container d-flex justify-content-between">
           <li>Home</li>
           <li>About</li>
           <li>Prices</li>
          </ul>
        </div>
      </nav>
  </header>
  
</template>

<script>

export default {
  name: 'HeaderComp',

}
</script>

<style lang="scss" scoped>
header{
  position: fixed;
  z-index: 10;
  top: 0;
  left: 0;
  width: 100%;
  .banner-top-nav{
    background-color: #353637;
    font-size: 12px;
    color: gray;
  }
  nav{
    background-color: rgba($color: #353637, $alpha: 0.5);
  }

}
  

</style>