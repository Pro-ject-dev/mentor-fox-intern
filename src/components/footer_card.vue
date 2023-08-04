<template>
    <div class="back">
      <p class="header">{{ header }}</p>
      <div class="content">
        <p class="para" v-for="item in itemList" :key="item.id">{{ item.text }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      itemList: {
        type: Array,
        required: true,
      },
      header:{
        type:String,
        required:true
      }
    },
  };
  </script>
  

<style scoped>

  .header{
    font-family: 'Unbounded';
    color:white;
    font-size: 20px;

}

.content{
    padding-top:2px;
    padding-left: 10px;
    font-family: 'Open Sans';
    font-size: 14px;
    color:white;

}

.back{
    width:30%
}

.para{
    padding: 10px;
}




</style>