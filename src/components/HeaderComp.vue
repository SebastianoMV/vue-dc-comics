<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="logo">
      <div>
        <ul>
          <li v-for="(item, index) in headerMenu" :key="index">
            <a :class="{'active': item.active == true}" href="item.href">{{item.name}}</a>
          </li>
          
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name:"HeaderComp",
  data(){
    return{
      headerMenu:[
        {
          name:'characters',
          href: '#',
          active: false,
        },
        {
          name:'comics',
          href: '#',
          active: true,
        },
        {
          name:'movies',
          href: '#',
          active: false,
        },
        {
          name:'tv',
          href: '#',
          active: false,
        },
        {
          name:'games',
          href: '#',
          active: false,
        },
        {
          name:'collectibles',
          href: '#',
          active: false,
        },
        {
          name:'videos',
          href: '#',
          active: false,
        },
        {
          name:'fans',
          href: '#',
          active: false,
        },
        {
          name:'news',
          href: '#',
          active: false,
        },
        {
          name:'shops',
          href: '#',
          active: false,
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utilities";
@import "../assets/style/var";


header{

  height: 100px;

  .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      width: 70px;
    }
    ul{
      display: flex;
      li{
        margin: 10px;
        a{
          font-weight: bold;
          color: black; 
          text-transform: uppercase;
          &:hover,
          &.active{
            color: $primary-color;
            text-decoration: underline;
            text-decoration-color: $primary-color;
          }
        }
        
      }
    }
  }
  
}
</style>