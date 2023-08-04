<template>
    <div class="card">
      <font-awesome-icon :icon="icon" flip="horizontal" size="xl" class="custom-icon" />
      <p class="heading">{{ heading }}</p>
      <p class="con-content">{{ content }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      icon: {
        type: Array,
        required: true,
      },
      heading: {
        type: String,
        required: true,
      },
      content: {
        type: String,
        required: true,
      },
    },
  };
  </script>


<style scoped>

@media (min-width:901px) {
  
.card{
    padding:10px;
    border:1px solid grey;
    border-bottom: 3px solid black;
    border-right:3px solid black;
    margin-bottom: 50px;
    }

    .heading{
        font-family: 'Unbounded';
        font-weight: 600;
    font-size: 16px;
    margin-bottom: 4px;
    }

    .con-content{
  width:400px;

        font-family: 'Open Sans';
        font-size: 10px;
        color:grey;
       margin-right: 20px;
    }
    .custom-icon{
    color: #dcff2e; 
        
        margin: 5px;
    }
    }



    @media (max-width:900px) {
  .card{
    padding:10px;
    border:1px solid grey;
    border-bottom: 3px solid black;
    border-right:3px solid black;
    margin-bottom: 20px;
    }

    .heading{
        font-family: 'Unbounded';
        font-weight: 600;
    font-size: 14px;
    margin-bottom: 4px;
    }

    .con-content{
       width:270px;
        font-family: 'Open Sans';
        font-size: 10px;
        color:grey;
       margin-right: 20px;
    }
    .custom-icon{
    color: #dcff2e; 
        
        margin: 5px;
    }
    
    }
</style>
  