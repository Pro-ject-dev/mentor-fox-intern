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
<p class="header">Your furniture's journey</p>
<p class="para">Furinture manufacturing is the process of designing, Creating and producing furniture.It involves a range of activities, including sourcing materials, creating designs, building prototypes, testing and refining products, and mass producing finished products</p>
</div >
<div class="cards">
<card :icon="['fas', 'file-arrow-up']" heading="Upload your inspiration"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />
        
<card :icon="['fas', 'gear']" heading="Customize your furniture"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card  :icon="['fas', 'tag']"  heading="Get your Quote"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />    

<card  :icon="['fas', 'percent']" heading="Confirm only with 50% advance"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card :icon="['fas', 'location-crosshairs']" heading="Track your furniture periodically"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

<card :icon="['fas', 'hand-holding-dollar']"  heading="Get Delivered"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />
                         
<card :icon="['fas', 'face-smile']" heading="You stunned right? we see your happy face"
                  content="Upload your inspiration with us and define your needs like comport, materials & colors, etc., and get your quote range" />

</div>
</div>
<div class="container">
  <div class="image-container">
    <img src="https://firebasestorage.googleapis.com/v0/b/mapview-aafa3.appspot.com/o/kl.jpg?alt=media&token=09fefa50-2a63-4d1d-9268-65cbf128c556">
  </div>
  <div class="glass"></div>
  <div class="cont"><p>Creating something for your own comfort is always a special experience.</p>  <button onclick="">Customize Now</button></div>
 
</div>


</template>



<style scoped>

@media (min-width:901px) {
.bg{
    display:flex;
    justify-content: space-between;
    align-items: start;
    max-width: 100%;
    height:150%;
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
  font-family: 'Open Sans';
  font-size: 13px;
    margin-top: 6px;
    width: 70%;
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
  display: flex;
}

.glass {
  align-items: end;
  justify-content: end;
  display: flex;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height:240px;
  background-color: rgba(0, 0, 0, 0.8);
}
.cont{
  width: 400px;
  margin:20px;
    position: absolute;
    top: 40px;
  left: 0;
  color:white;
  font-size: 20px;
  font-family:'Unbounded';
  font-weight: 500;
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
}




@media (max-width:900px) {
  .bg{
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
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
    font-size: 21px;
    width:250px;
}
.para{
  font-family: 'Open Sans';
  font-size: 12px;
    margin-top: 6px;
    margin-bottom: 30px;
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
  background-color: rgba(0, 0, 0, 0.8);
}




.cont{
  margin:20px;
  position: absolute;
  top:20px;
  left:0;
  color:white;
  font-size: 20px;
  font-family:'Unbounded';
  font-weight: 500;
}

button {
  padding:10px;
  position: absolute;
  top: 140px;
  left: 0;
  color:black;
  background-color: rgb(255, 247, 0);
  font-size: 10px;
  font-family: 'Unbounded';
  font-weight: 700;
  border: 0px;
  display: block;
  margin: 0 auto;
}
}


</style>
