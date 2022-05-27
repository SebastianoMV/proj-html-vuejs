<template>
  <header>
      <div class="banner-top-nav">
        <div class="container d-flex justify-content-between py-2">
          <span>We have a 95% Successful Pass Rate!</span>
          <span>Give us a call</span>
        </div>
      </div>
      <nav>
        <div class="container d-flex py-4">
          <img src="../assets/img/avada-drivers-logo-2x-400x77.png" alt="avada drivers logo">
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
  z-index: 998;
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
    color: white;
    height: 100px;
    img{
      width: 20%;
    }
    ul{
      width: 75%;
      list-style: none;
      margin: auto;
    }
  }

}
  

</style>