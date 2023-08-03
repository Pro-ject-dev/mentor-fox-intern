<template>

<div class="bg">
    <p class="header">Hear what our </p>
    <p class="header"> happy customers say</p>
    <div class="cards">
    <card1 name="Jeevan Raj" city="Mumbai"/>
    <card1 name="Rahul" city="Mumbai"/>
    <card1 name="Karthick" city="Mumbai"/>
    </div>
</div>

</template>

<script>
import card1 from './card1.vue'
export default{
    name:'card2',
    components:{
        card1
    }
}
</script>

<style scoped>
.header{
    display:flex;
    align-items: center;
    justify-content: center;
    font-weight: w600;
    font-family: 'Unbounded';
    font-size: 25px;
    color:rgb(51, 0, 55);

}
.bg{
    margin-top:30px;
height:500px;
padding:20px;
}

.cards{
    display: flex;
    padding:20px;
}



</style>
