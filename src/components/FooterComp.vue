<template>
  <footer>
      <!-- MAIN FOOTER -->
      <div class="main-footer">
        <div class="container">
          <div class="ul-container-footer">
            <div>
                <h2>DC COMICS</h2>
                <ul>
                  <li><a href="#">Characters</a></li>
                  <li><a href="#">Comics</a></li>
                  <li><a href="#">Movies</a></li>
                  <li><a href="#">TV</a></li>
                  <li><a href="#">Games</a></li>
                  <li><a href="#">Video</a></li>
                  <li><a href="#">News</a></li>
              
                </ul>
                <h2>SHOP</h2>
                <ul>
                  <li><a href="#">Shop DC</a></li>
                  <li><a href="#">Shop DC Collectibles</a></li>
                  
                </ul>
            </div>
            <div>
              <h2>DC</h2>
              <ul>
                  <li><a href="#">Terms Of Use</a></li>
                  <li><a href="#">Privacy policy (New)</a></li>
                  <li><a href="#">Ad Choises</a></li>
                  <li><a href="#">Advertising</a></li>
                  <li><a href="#">Jobs</a></li>
                  <li><a href="#">Subscriptions</a></li>
                  <li><a href="#">Talent Workshops</a></li>
                  <li><a href="#">CPSC Certificates</a></li>
                  <li><a href="#">RAtings</a></li>
                  <li><a href="#">Shop Help</a></li>
                  <li><a href="#">Contact Us</a></li>
              
                </ul>
            
            </div>
            <div>
              <h2>SITES</h2>
              <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
                
              </ul>

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
      padding-top: 20px;
      width: 40%;
      height: 100%;
      display: flex;
      justify-content: space-between;
      color: white;
      h2{
        margin-bottom: 20px;
        margin-top: 20px;
      }
      ul li{
          margin-top: 5px;
        } 
        a{
          color: rgb(174, 172, 172);
          
          
        }
      
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
      color: $primary-color;
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