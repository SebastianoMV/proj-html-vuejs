<template>
<div>
    <VueSlickCarousel :dots="true">
      <div v-for="(testimonial, index) in testimonialsArr" :key="index">
        <img class="my-3" :src="testimonial.img" alt="">
        <p>{{testimonial.text}}</p>
        <h4>{{testimonial.name}}</h4>
      </div>
    </VueSlickCarousel>
  </div>
  
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
  export default {
  name: 'CarouselComp',
  components: { VueSlickCarousel },
  data() {
    return {
      testimonialsArr:[
        {
          name: 'Sophia Jones',
          img:require('../assets/img/testimonial-sophia.png'),
          text:'Avada Driving School really helped my confidence behind the weel and with drivingin general, and they got my a first time pass! Highly raccomanded'
        },
        {
          name: 'Grant Qualcosa',
          img:require('../assets/img/testimonial-grant.png'),
          text:'Avada Driving School really helped my confidence behind the weel and with drivingin general, and they got my a first time pass! Highly raccomanded'
        },
        {
          name: 'Harold Ebbasta',
          img:require('../assets/img/testimonial-harold.png'),
          text:'Avada Driving School really helped my confidence behind the weel and with drivingin general, and they got my a first time pass! Highly raccomanded'
        },
        {
          name: 'Kate Perry',
          img:require('../assets/img/testimonial-kate.png'),
          text:'Avada Driving School really helped my confidence behind the weel and with drivingin general, and they got my a first time pass! Highly raccomanded'
        },
        {
          name: 'Kelly De Kelly',
          img:require('../assets/img/testimonial-kelly.png'),
          text:'Avada Driving School really helped my confidence behind the weel and with drivingin general, and they got my a first time pass! Highly raccomanded'
        },
      ]
    }
  },
  

}
</script>

<style>
.slick-dots li button:before{
  font-size: 15px;
}
img{
  width: 20%;
  margin: auto;
}

</style>