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

  data(){
    return{
      headFooterMenu: [
        {
          name:'digital comics',
          href: '#',
          image: '../assets/img/buy-comics-digital-comics.png',
        },
        {
          name:'dc merchandise',
          href: '#',
          image: '../assets/img/buy-comics-digital-comics.png',
        },
        {
          name:'subscription',
          href: '#',
          image: '../assets/img/buy-comics-digital-comics.png',
        },
        {
          name:'comic shop locator',
          href: '#',
          image: '../assets/img/buy-comics-digital-comics.png',
        },
        {
          name:'dc power visa',
          href: '#',
          image: '../assets/img/buy-comics-digital-comics.png',
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
      width: 100%;
      display: flex;
      align-items: center;
      list-style: none;
      justify-content: space-around;
      li{
        display: flex;
        align-items: center;
        a{
          color: white;
          text-decoration: none; 
          text-transform: uppercase;
          margin-left: 10px;
        }
      }
      
    }
}
img{
  width: 40px;
}

</style>