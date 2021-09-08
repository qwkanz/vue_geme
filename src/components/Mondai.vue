<template>
  <div class="alert alert-info">
    <h2 class=text-warning>{{title}}</h2>
    <p class="text-success">{{message}}</p>


    
  </div>
</template>

<script>
export default{
  name: 'mondai',
  props :{
    title: String,
    answer :String,
    message: String,
   
  }
}
</script>

<style >
 
</style>