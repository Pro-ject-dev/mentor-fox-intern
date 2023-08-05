<template>
    <div class="back">
      <div class="head">
      <p class="header">{{ header }}</p>
    </div>
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

@media (min-width: 900px) {
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

}

@media (max-width:901px) {
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

/* .head{
  width:80%;
  
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: start;
} */
.back{
  justify-content: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top:50px;
    width:80%
}

.para{
    padding-top: 20px;
    
}

}

  



</style>