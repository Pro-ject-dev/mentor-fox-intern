<template>
<div class="bgb">
<img :src="images">
<p class="head">{{ header }}</p>
<p class="para">{{ contents }}</p>
<div class="horizontal-line"></div>

<div class="foot">
<p  class="date">{{ date }}</p>

<div class="read">
    <p>Read More</p>
<font-awesome-icon :icon="['fas', 'arrow-right']" />
</div>

</div>
</div>
</template>

<script>
export default{
    name:'card2',
    props:{
        header:{
            type:String,
            required:true

        },
    contents:{
    type:String,
    required:true
},
    images:{
    type:String,
    required:true
},
    date:{
   type:String,
   required:true 
}
    
}
}
</script>

<style scoped>
img{
    width: 300px;
    height:200px;
}
.bgb{
  
height:60%;
margin:40px;
    padding:20px;
    border:1px solid black;
    }
.head{
    margin-top: 5px;
    font-size: 16px;
    font-family: 'Unbounded';
    font-weight: 600;
}

.para{
    padding-top: 10px;
    font-family: 'Open Sans';
    font-size: 10px;
    font-weight: 500;
}

.horizontal-line {
    padding: 10px;
    width: 300px;
    margin-bottom: 10px;
  border-bottom: 1px solid grey;
}

.read{
    display: flex;
 margin: 8px;
 padding:8px;
  height: 2.3rem;
  width: 6rem;
  background-color: rgb(255, 247, 0);
  font-size: 13px;
  font-family:'Roboto Condensed' ;
  font-weight: 800;
  border: 0px;
  align-items: center;
  justify-content: space-between;
}

.date{
    font-size: 11px;
    font-family: 'Open Sans';
}

.foot{
width:300px;
    align-items: center;
    justify-content:space-between;
    display: flex;
}


  
</style>