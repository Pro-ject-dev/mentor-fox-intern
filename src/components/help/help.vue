<template>
<div class="bg">
<p>Need help in choosing the best?</p>
<div class="cards">
    <card3 header="Here's how to choose the right sofa"  contents="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023" images="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/jk.png?alt=media&token=d51567b6-d1ca-44a1-bd21-d04eeaed05ff"/>
    <card3 header="Here's how to choose the right sofa"  contents="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023 " images="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/kj.png?alt=media&token=2fb40cac-8943-4195-b614-85c7dbf3d6d1"/>
    <card3 header="Here's how to choose the right sofa"  contents="Selecting a sofa is one of the most important furnishing decisions you can make! Think about it - so much of your home life centers around this one piece. Relaxing after wor..." date="16 Jan, 2023 "  images="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/op.png?alt=media&token=46802562-b3db-47a1-ae4b-de7938c14738"/>


</div>
</div>
</template>

<script>
import card3 from '../help_card.vue'

export default{
    name:'screen7',
    components:{
        card3
    }
}
</script>

<style scoped>

@media (min-width:901px){
.bg{
justify-content: center;
align-items: center;
display: flex;
flex-direction: column;
padding:30px 0px 0px 0px;
}

p{

    font-size: 24px;
    font-weight: 500 ;
    font-family: 'Unbounded';

}

.cards{
   
    display: flex;
}
}

@media (max-width: 900px) {
  .bg{
justify-content: center;
align-items: center;
display: flex;
flex-direction: column;
padding:30px;
}

p{

    font-size: 15px;
    font-weight: 500 ;
    font-family: 'Unbounded';
    font-weight: 600;

}

.cards{

    display: flex;
    max-width: 120%;
  overflow-x: auto; 

}
}  


</style>