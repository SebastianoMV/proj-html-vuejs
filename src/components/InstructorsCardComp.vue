<template>
<div class="row">
<div class="col border-top-green mx-1 box-white-standard position-relative" v-for="(instructor, index) in instructors" :key="`inst-${index}`" >
  <div class="text-center p-5">
    <img :src="instructor.image" alt="blog post">
    <h4>{{instructor.name}}</h4>
    <div> 
      <i class="fa-brands fa-facebook-f mx-2"></i>
      <i class="fa-brands fa-twitter mx-2"></i>
      <i class="fa-brands fa-instagram mx-2"></i>
    </div>
    <p>{{instructor.text}}</p>
  </div>
  <div class="hover-card-message">instructor: {{instructor.name}}</div>
</div>
</div>
</template>

<script>
export default {
  name: 'InstructorsCardComp',
  data() {
    return {
      instructors:[
        {
          name:'Mike Hart',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta.',
          image: require('../assets/img/instructor-mikehart.jpg')
        },
        {
          name:'John Smith',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta.',
          image: require('../assets/img/instructor-johnsmith.jpg')
        },
        {
          name:'Angela Hart',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta.',
          image: require('../assets/img/instructor-angelahart.jpg')
        },
      ]
    }
  },

}
</script>

<style lang="scss" scoped>
  h4{
    color: black;
  }
  img{
    width: 100%;
  }
  .hover-card-message{
    background-color: white;
    border: 1px solid black;
    padding: 5px;
    position: absolute;
    top: 200px;
    left: 50%;
    display: none;
  }
  .col:hover{
    transform: scale(1, 1.05);
  }
 .col:hover .hover-card-message{
     display: inline-block;
  }

</style>