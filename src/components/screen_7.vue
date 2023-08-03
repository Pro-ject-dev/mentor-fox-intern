<template>
<div class="bg">
<p>Need help in choosing the best?</p>
<div class="cards">
    <card3 header="Here's how to choose the right sofa"  content="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023 "/>
    <card3 header="Here's how to choose the right sofa"  content="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023 "/>
    <card3 header="Here's how to choose the right sofa"  content="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023 "/>


</div>
</div>
</template>

<script>
import card3 from './card2.vue'

export default{
    name:'screen7',
    components:{
        card3
    }
}
</script>

<style scoped>

.bg{
justify-content: center;
align-items: center;
display: flex;
flex-direction: column;
padding:30px;
}

p{

    font-size: 24px;
    font-weight: 500 ;
    font-family: 'Unbounded';

}

.cards{
   padding:10px;
    display: flex;
}


</style>