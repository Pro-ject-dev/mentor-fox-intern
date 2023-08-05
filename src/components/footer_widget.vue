
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



@media (min-width: 901px) {
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
    align-items: center;
    color: white;
margin-left: 20px;

}
}

@media (max-width:900px){
  img{
    height:40px;
    width:40px;
}

.first{
    display: flex;
    width: 100%;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    
   
}
.ph{
  margin-top:5px;
    font-family: 'Open Sans';
    color:gray;
    font-size: 15px;
    
}

.phno{
    padding-top: 5px;
    font-family: 'Unbounded';
    color:rgb(255, 255, 255);
    font-size: 10px;
}


.cont{
    
    display: flex;
    flex-direction: column;
    color: white;
align-items: center;

}
}

</style>
  