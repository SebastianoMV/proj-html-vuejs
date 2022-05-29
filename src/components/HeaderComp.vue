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
           <li>Courses <span>new</span></li>
           <li>locations</li>
           <li>blog</li>
           <li><BtnComp btnString="book now"/></li>
          </ul>
        </div>
      </nav>
  </header>
  
</template>

<script>
import BtnComp from './BtnComp.vue';

export default {
    name: "HeaderComp",
    components: { BtnComp }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/var';
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
    background-color: rgba($color: #353637, $alpha: 0.7);
    color: white;
    height: 100px;
    img{
      width: 20%;
    }
    ul{
      width: 75%;
      list-style: none;
      margin: auto;
      span{
        background-color: $primary-color;
        border-radius: 5px;
        padding: 2px 5px;
        font-size: 10px;
      }
      li{
        text-transform: uppercase;
        margin: auto;
      }
    }
  }

}
  

</style>