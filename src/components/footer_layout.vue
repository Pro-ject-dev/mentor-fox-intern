
<template>
    <div class="first">
      <img :src="imageSrc" alt="">
      <div class="cont">
        <p class="ph">{{ title }}</p>
        <p class="phno">{{ phoneNumber }}</p>
      </div>
    </div>
  </template>
  
  <script>
  
  export default {
    props: {
      imageSrc: String,
      phoneNumber: String,
      title:String
    }
  }
  </script>


<style scoped>




img{
    height:35px;
    width:35px;
}

.first{
    display: flex;
    margin-right: 60px;
   
}
.ph{
    font-family: 'Open Sans';
    color:gray;
    font-size: 12px;
    
}

.phno{
    padding-top: 5px;
    font-family: 'Unbounded';
    color:rgb(255, 255, 255);
    font-size: 12px;
}


.cont{
    
    display: flex;
    flex-direction: column;
    color: white;
margin-left: 20px;

}
</style>
  