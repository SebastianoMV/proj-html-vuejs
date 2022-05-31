<template>
  <header>
      <div class="banner-top-nav">
        <div class="container d-flex justify-content-between py-2">
          <span>We have a 95% Successful Pass Rate!</span>
          <span><i class="fa-solid fa-phone-flip"></i> Give us a call to book your tuition! 1-880-555-555</span>
        </div>
      </div>
      <nav>
        <div class="container d-flex py-4">
          <img src="../assets/img/avada-drivers-logo-2x-400x77.png" alt="avada drivers logo">
          <ul class="container d-flex justify-content-between">
           <li v-for="(item, index) in headerMenu" :key="index">
            <div :class="{'activenav': item.active == true}" @click="activeClick(index)">{{item.name}} <span v-if="item.new != ''">{{item.new}}</span></div>
           </li>
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
    components: { BtnComp },
    data() {
      return {
        active: true,
        headerMenu:[
        {
          name:'home',
          href: '',
          active: true,
          new: '',
        },
        {
          name:'about',
          href: '',
          active: false,
          new: '',
        },
        {
          name:'prices',
          href: '',
          active: false,
          new: '',
        },
        {
          name:'courses',
          href: '#',
          active: false,
          new: 'new',
        },
        {
          name:'locations',
          href: '#',
          active: false,
          new: '',
        },
        {
          name:'blog',
          href: '#',
          active: false,
          new: '',
        },
        
      ]
      }
    },
    methods: {
      activeClick(n){
        this.headerMenu[n].active = !this.headerMenu[n].active;
      }
    },
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
    // position: sticky;
    // top: 0px;
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
        a{
          text-decoration: none;
          color: white;
        }
      }
    }
  }

}
  

</style>