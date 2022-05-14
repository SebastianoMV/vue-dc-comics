<template>
  <div class="head-footer">
        <div class="container">
          <ul>
          <li v-for="(item, index) in headFooterMenu" :key="index">
            <img v-bind:src="item.image" alt="">
            <a>{{item.name}}</a>
          </li>
          
        </ul>
       
        </div>

      </div>
</template>

<script>
export default {
  name: "BannerComp",

  mounted(){
    console.log(this.headFooterMenu[0].image);
  },

  data(){
    return{
      headFooterMenu: [
        {
          name:'digital comics',
          href: '#',
          image: require('../assets/img/buy-comics-digital-comics.png'),
        },
        {
          name:'dc merchandise',
          href: '#',
          image: require('../assets/img/buy-comics-merchandise.png'),
        },
        {
          name:'subscription',
          href: '#',
          image: require('../assets/img/buy-comics-subscriptions.png'),
        },
        {
          name:'comic shop locator',
          href: '#',
          image: require('../assets/img/buy-comics-shop-locator.png'),
        },
        {
          name:'dc power visa',
          href: '#',
          image: require('../assets/img/buy-dc-power-visa.svg'),
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utilities";
@import "../assets/style/var";

.head-footer{
  height: 150px;
  background-color: $primary-color;
}
.container{
  display: flex;
  height: 100%;
  
  ul{
    margin: 30px;
      width: 100%;
      display: flex;
      align-items: center;
      li{
        display: flex;
        width: 100%;
        align-items: center;
        a{
          color: white;
          text-transform: uppercase;
          margin-left: 5px;
          width: 100%;
          
        }
      }
      
    }
}
img{
  max-width: 40px;
  max-height: 40px;
}

</style>