<template>
  <div class="bg">
    <div class="background-img">
      <p class="c1">From Concept to creation, we bring your furniture dream to life</p>
      <p class="c2">We specialize in creating unique, one-of-a-kind pieces tailored furniture</p>
      <button>Customize Now</button>
    </div>
    </div>
  </template>
  
  
  <script>

  
  export default {
    name: 'img',
  };
  </script>
  
  <style scoped>

.bg{
  min-width: 100%;
}


.background-img{
background-image:url("https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/WhatsApp%20Image%202023-08-01%20at%209.32.32%20PM.jpeg?alt=media&token=84d3b0e7-c803-455c-ade1-68ee696dc90d") ;
background-repeat: no-repeat;
background-size: cover;
align-items: center;
justify-content: center;
display: flex;
flex-direction: column;
width:100%;
padding:20%;
}



.c1{
  font-weight: 600;
  display: flex;
  text-align: center;
  justify-content: center;
  align-items: center;
  font-family: 'Unbounded';
  color:white;
  font-size:31px;
}

.c2{
  font-size:15px;
  color:white;
  padding-top:10px;
  padding-right:10px;
  padding-bottom:10px;
  font-family: 'Open Sans';

}

button{
font-weight: 600;
padding:10px 30px ;
background-color: yellow;
border: 0px;
font-size: 12px;
font-family: 'Unbounded';
}

@media screen and (max-width: 900px) {
  .c1{
  font-weight: 600;
  display: flex;
  text-align: start;
  font-family: 'Unbounded';
  color:white;
  font-size:21px;
}
.background-img{
background-image:url("https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/WhatsApp%20Image%202023-08-01%20at%209.32.32%20PM.jpeg?alt=media&token=84d3b0e7-c803-455c-ade1-68ee696dc90d") ;
background-repeat: no-repeat;
background-size: cover;
align-items: start;
justify-content: start;
display: flex;
flex-direction: column;
width:100%;
padding:5%;
padding-top: 38%;

}
.c2{
  font-size:11px;
  color:white;
  padding-top:10px;
  padding-bottom:10px;
  font-family: 'Open Sans';

}
}


</style>


  