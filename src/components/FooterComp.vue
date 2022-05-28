<template>
  <footer>
    <!-- FOOTER -->
    <div class="footer-bg background-cover">
      <div class="debug container">
        <div class="row">
          <div class="col debug"></div>
          <div class="col debug"></div>
          <div class="col debug"></div>
          <div class="col debug"></div>
        </div>
      </div>
    </div>

     <!-- BANNER COPY -->
    <div class="copy-bg background-cover">
      <div class="debug container">
        BANNER COPY
      </div>
    </div>
  </footer>
  
</template>

<script>
export default {
  name:'FooterComp'

}
</script>

<style lang="scss" scoped>
  .footer-bg{
    background-image: url(../assets/img/footer-background-color.jpg);
  }

  .copy-bg{
    background-color: black;
  }

</style>