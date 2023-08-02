<script>
import card from './card.vue'

export default{
    name:'screen4',

    components:{
        card
    }
}
</script>

<template>

<div class="bg">
<div class="contents">
<p class="header">Your furniture's <br> journey</p>
<p class="para">Furinture manufacturing is the process of designing, Creating and producing<br>furniture.It involves a range of activities, including sourcing materials, creating <br> designs, building prototypes, testing and refining products, and mass producing <br>finished products</p>
</div >
<div class="cards">
<card :icon="['fas', 'file-arrow-up']" heading="Upload your inspiration"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />
        
<card :icon="['fas', 'file-arrow-up']" heading="Customize your furniture"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card :icon="['fas', 'file-arrow-up']" heading="Get your Quote"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />    

<card :icon="['fas', 'file-arrow-up']" heading="Confirm only with 50% advance"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card :icon="['fas', 'file-arrow-up']" heading="Track your furniture periodically"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card :icon="['fas', 'file-arrow-up']" heading="Get Delivered"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />
                         
<card :icon="['fas', 'file-arrow-up']" heading="You stunned right? we see your happy face"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

</div>
</div>
<div class="container">
  <div class="image-container">
    <img src="https://firebasestorage.googleapis.com/v0/b/mapview-aafa3.appspot.com/o/kl.jpg?alt=media&token=09fefa50-2a63-4d1d-9268-65cbf128c556">
  </div>
  <div class="glass"></div>
  <div class="cont"><p>Creating something for your<br>own comfort is always a <br> special experience.</p>  <button onclick="">Customize Now</button></div>
 
</div>
<div class="y">

</div>

</template>



<style scoped>
.bg{
    display:flex;
    justify-content: space-between;
    align-items: start;
    max-width: 100%;
    height:170%;
    padding:25px;
    padding-top:12%;
    background-color: white;  
 
}

.contents{

    display:inline;
    justify-content: start;
    align-items: start;
}

.header{
    font-family: 'Unbounded';
    font-size: 23px;
}
.para{
    margin-top: 6px;
    color: grey;
}
.cards{
    display:inline;
    padding-bottom: 30px;
    margin-bottom: 20px;
}


.container {
  position: relative;
}

.image-container img {
  width: 100%;
  height: 230px;
  display: block;
}

.glass {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height:240px;
  background-color: rgba(0, 0, 0, 0.8); /* Set the desired background color and opacity for the "glass" div */
}




.cont{
    margin: 70px;
    position: absolute;
    top: 0;
  left: 0;
  color:white;
  font-size: 21px;
  font-family:'Unbounded';
  font-weight: 600;
}

button {
    position: absolute;
    top: 100px;
  left: 0;
  height: 2.3rem;
  width: 10rem;
  color:black;
  background-color: rgb(255, 247, 0);
  font-size: 12px;
  font-family: 'Unbounded';
  font-weight: 700;
  border: 0px;
  display: block;
  margin: 0 auto;
}

.y{
    height:700px;
}

</style>
