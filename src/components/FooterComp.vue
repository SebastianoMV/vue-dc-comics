<template>
  <footer>
      <!-- MAIN FOOTER -->
      <div class="main-footer">
        <div class="container">
          <div class="ul-container-footer">
            <div>
                <h2>DC COMICS</h2>
                <h2>SHOP</h2>
            </div>
            <div>
              <h2>DC</h2>
            
            </div>
            <div>
              <h2>SITES</h2>

            </div>

          </div>

          <div class="logo-bg">

          </div>
        </div>

      </div>

      <!-- FOOT FOOTER -->
      <div class="foot-footer">
        <div class="container">
          <div class="btn-footer">
            <a href="#"> SING-UP NOW!</a>
          </div>
          <div class="social">
            <h2>FOLLOW US</h2>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
          </div>
        </div>

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
    .ul-container-footer{
      width: 40%;
      height: 100%;
      display: flex;
      justify-content: space-between;
      color: white;
    }
  }
  
}

.foot-footer{
  height: 100px;
  background-color: #303030;
  .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .btn-footer{
      border: 2px solid $primary-color;
      padding: 10px;
      a{
        text-decoration: none;
        color: white;
      }
       
    };
    .social{
      display: flex;
      align-items: center;
      img{
        margin-left: 15px;
      }
    }
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