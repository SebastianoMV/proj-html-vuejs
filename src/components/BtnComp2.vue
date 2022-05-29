<template>
<div>
  <a class="btnsmv">{{btnString}}</a>
</div>

  
</template>

<script>
export default {
  name: 'BtnComp2',
  props:{
    btnString: String,
  }
}
</script>

<style lang="scss" scoped>

.btnsmv{
  display: inline-block;
  border-radius: 50px;
  padding: 5px 20px;
  border: 3px solid;
  border-color: #7094a9;
  color: #7094a9;
  text-decoration: none;
  text-transform: uppercase;
  font-weight: 600;
  
  
  &:hover{
    background-color: white;
    color: #7094a9;
  }
  

}

</style>