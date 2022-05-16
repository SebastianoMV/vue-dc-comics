<template>
   <div class="card"> 
     <div class="card-img">
       <img :src="card.thumb" :alt="card.series">
     </div>
     <h5>{{card.series}}</h5>
    </div>
      
   
</template>

<script>

export default {
  name: "CardComp",
  props:{
    card:Object,
  },
}
</script>

<style lang="scss" scoped>

.card{
  margin-top: 40px;
  .card-img{
    overflow: hidden;
    width: 200px;
    height: 200px;
  }
  h5{
    margin-top: 10px;
    text-transform: uppercase;
    width: 200px;
  }
  
}

</style>