<template>
  <div>
    <HeaderComp/>
    <JumboComp/>
    <MainComp/>
    <FooterComp/>
    
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';
import JumboComp from './components/JumboComp.vue';


export default {
    components: { HeaderComp, MainComp, FooterComp, JumboComp }
}
</script>

<style lang="scss">
@import './assets/style/general';
@import './assets/style/utilities'

</style>
