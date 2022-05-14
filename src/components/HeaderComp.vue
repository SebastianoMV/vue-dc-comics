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
      align-items: center;
      height: 100px;
      li{
        margin: 10px;
        height: 100%;
        a{
          display: flex;
          align-items: center;
          height: 100%;
          font-weight: bold;
          color: black; 
          text-transform: uppercase;
          border-bottom: 4px solid transparent;
          &:hover,
          &.active{
            color: $primary-color;
            border-bottom: 4px solid $primary-color;
            
          }
        }
        
      }
    }
  }
  
}
</style>