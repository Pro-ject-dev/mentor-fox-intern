<template>
<div class="card">

<div class="circle-avatar">
    <font-awesome-icon class="icon" :icon="['fas', 'quote-left']" />
</div>

<div class="contents">
     <p class="head">You Stunned right? we see your<br>happy face</p>
     <p class="para">upload your inspiraton with us  and define your needs <br> like comport, materials & colors,etc.,and get your quote<br>range.</p>
</div>

<div class="horizontal-line"></div>

<div class="name-city">
    <p class="head">{{name}}</p>
    <p class="para">{{ city }}</p>
</div>

</div>
</template>

<script>
export default{
    name:"card2",
    props:{
name:{
    type:String,
    required:true,
},
city:{
    type:String,
    required:true, 
}

}
}

</script>

<style scoped>
.card{
    align-items: center;
    justify-content: center;
    height:280px;
    width:360px;
    padding:20px;
    margin:20px;
    border:1px solid rgb(193, 193, 193);
}

.circle-avatar{
  justify-content: "center";
  display: flex;
  padding:8px;
   align-items: center;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    background-color: rgb(72, 3, 77);
}

.para{
font-family: 'Open Sans';
font-size: 12px;
color:grey
}


.icon {
  font-size: 24px; 
  color: #ffffff;
}

.head{
    font-weight: 600;
    font-family: 'Unbounded';
    font-size: 16px;
    margin-bottom: 7px;
color:rgb(72, 3, 77);
}

.contents{
    margin-top: 16px;
    margin-bottom: 8px;
}

.horizontal-line {
    padding: 10px;
    margin-bottom: 20px;
    border-bottom: 1px solid rgb(193, 193, 193);
}




</style>