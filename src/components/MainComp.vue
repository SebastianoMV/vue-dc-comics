<template>
  <main>
    <div class="jumbo">
      <div class="container">
        <div class="btn-jumbo">Current Series</div>
      </div>
    </div>
    <div class="container">
      <CardComp v-for="(card,index) in dataDc" :key="index" :card="card"/>
    </div>
    <div class="btn-container">
      <div class="btn-more">Load more</div>
    </div>
    
    
 
   
  </main>
</template>

<script>
import CardComp from './CardComp.vue';
import dataDc from '../assets/data/dataDc'

export default {
    name: "MainComp",
    components: { CardComp },
    data(){
      return{
        dataDc
      }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/utilities";
@import "../assets/style/var";
  main{
    background-color: #1c1c1c;
    .container{
      display: flex;
      flex-wrap: wrap;
      padding-bottom: 20px;
    }
    color: white;
    .jumbo{
      position: relative;
      height: 400px;
      background-image: url(../assets/img/jumbotron.jpg);
      .btn-jumbo{
        position: absolute;
        bottom: -20px;
        padding: 10px 20px;
        background-color: $primary-color;
        text-transform: uppercase;
        font-weight: bold;
      }
    }
    .btn-container{
      padding: 30px;
    }
    .btn-more{
      width: 120px;
      padding: 10px 20px;
      background-color: $primary-color;
      text-transform: uppercase;
      font-weight: bold;
      margin: auto;
      margin-top: 20px;
    }
  }
</style>