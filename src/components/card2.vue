<template>
<div class="bg">
<img src="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/jk.png?alt=media&token=d51567b6-d1ca-44a1-bd21-d04eeaed05ff">
<p class="head">Here's how to choose the right sofa</p>
<p class="para">Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor...</p>
<div class="horizontal-line"></div>

<div class="foot">
<p  class="date">16 jan,2023</p>

<div class="read">
    <p>Read More</p>
<font-awesome-icon :icon="['fas', 'arrow-right']" />
</div>

</div>
</div>
</template>

<script>
export default{
    name:'card2'
}
</script>

<style scoped>
img{
    width: 300px;
    height:200px;
}
.bg{
height:60%;
margin:40px;
    padding:2px;
    border:1px solid black;
    width: 320px;
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