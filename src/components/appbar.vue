<template>
    <div class="appbar">
        <div class ="l-icon">
            <font-awesome-icon :icon="['fas', 'bars']" class="icon-left" />
        </div>
        <div class="content">
            <p class="text">BEST WOODS</p>
        </div>
        <div class="r-icon">
      <font-awesome-icon icon="magnifying-glass" class="icon-right" />
      <font-awesome-icon :icon="['fas', 'bell']" class="icon-right" style="color: #000000;" />
      <font-awesome-icon :icon="['fas', 'circle-user']" class="icon-right" />
      <font-awesome-icon :icon="['fas', 'cart-shopping']" class="icon-right" />
        </div>
    </div>
  
  </template>
  
  <style scoped>
@import url('https://fonts.googleapis.com/css?family=Unbounded');

.text{
font-family: 'Unbounded';
font-size: 15px;
}
  .appbar {
    display: flex;
    align-items: center;
    justify-content: space-between; 
    border: 1px solid grey;
    padding: 20px;
    font-size: 20;
    font-weight: 700;
  }
  
  .icon-left {
    margin-right: 10px;
  }
  
  .icon-right {
    margin-left: 10px;
    padding-left: 5px;
  }
 

  </style>
  