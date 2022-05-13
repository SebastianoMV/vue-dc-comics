<template>
  <footer>
      <!-- MAIN FOOTER -->
      <div class="main-footer">
        <div class="container">
          <div>

          </div>
          <div class="logo-bg">

          </div>
        </div>

      </div>

      <!-- FOOT FOOTER -->
      <div class="foot-footer">
        <div class="container"></div>

      </div>
    
  </footer>
</template>

<script>
export default {
  name:"FooterComp",
  
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utilities";
@import "../assets/style/var";

.main-footer{
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  .container{
    display: flex;
    justify-content: space-between;
    height: 100%;
  }
  
}




.logo-bg{
  height: 100%;
  width: 40%;
  background-image: url(../assets/img/dc-logo-bg.png);
  background-position: center;
  background-size: cover;
}

</style>