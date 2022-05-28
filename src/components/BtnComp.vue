<template>
<div>
  <a class="btnsmv">{{btnString}}</a>
</div>

  
</template>

<script>
export default {
  name: 'BtnComp',
  props:{
    btnString: String,
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/var';

.btnsmv{
  display: inline-block;
  border-radius: 50px;
  padding: 5px 20px;
  background-color: $primary-color;
  border: 2px solid;
  border-color: $primary-color;
  color: white;
  text-decoration: none;
  text-transform: uppercase;
  
  &:hover{
    background-color: white;
    color: $primary-color;
  }
  

}

</style>