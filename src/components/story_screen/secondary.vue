

<script>

export default{
    name:'secondary',
}
</script>
<template>
    <div class="contents">
    <div class="image">
    <img src="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/WhatsApp%20Image%202023-08-02%20at%202.28.59%20PM.jpeg?alt=media&token=d157f3a4-9b86-4b3e-8270-c45aec7b4ef3">
    </div>
    <div class="lines">
        <p>The timeless luxury of</p>
        <p>custom design</p>
        <div class="para">
<p class="cont">
    Best Woods Furniture speacializes in crafting high-quality, custom furniture for a variety of clients including individuals, interior designers, and commercial properties. We offer full-service manufacturing  and design services to bring your vision to life.
</p>
</div>
<div class="story">
<p>Our Story</p>
<font-awesome-icon :icon="['fas', 'arrow-right']" />
</div>

        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Roboto+Condensed');
@import url('https://fonts.googleapis.com/css?family=Open+Sans');

.image{
    width:100%;
  
}
img{
    width:100%;
    height:700px;
}


.contents{
    padding: 0px;
    margin: 0px;
    display: flex;
    align-items: center;
    background-color: whitesmoke;
    font-size: 45px;
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}

.lines{
    display:inline;
}

.para{
    padding: 5px;
    font-weight: 500;
    font-family: 'Open Sans';
    color:grey;
    font-size: 10.5px;
}
p{
    padding:2px;
   
}

.cont{
    padding-right:30px
}
.story{
    display: flex;
 margin: 8px;
 padding:8px;
  height: 2.3rem;
  width: 10rem;
  background-color: rgba(229, 222, 12, 0.5);
  font-size: 20px;
  font-family:'Roboto Condensed' ;
  font-weight: 800;
  border: 0px;
  align-items: center;
  justify-content: space-between;
}

@media screen and (max-width: 900px) {
    .contents {
        padding-left:8px;
        padding-top: 20px;
        margin: 0px;
        display: grid;
        justify-content: start;
        justify-items: start;
        background-color: whitesmoke;
        font-size: 22px;
        font-family: 'Unbounded';
        grid-template-areas: "lines" ; 
    }

    .lines{
        grid-area: lines;
    }

    img{
    grid-area:img;
    width:100%;
   height:400px

    }

.story{
    display: flex;
 margin: 8px;
 padding:10px;
  background-color: rgba(229, 222, 12, 0.5);
  font-size: 15px;
  font-family:'Roboto Condensed' ;
  font-weight: 800;
  border: 0px;
  align-items: center;
  justify-content: space-between;
}
    
   
}


</style>