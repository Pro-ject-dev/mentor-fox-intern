<template>
    <div class="container">
      <div class="image-container">
        <img src="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/wall-416060_1280.jpg?alt=media&token=a368812c-7e12-4f06-9566-ade680c1e3b3">
      </div>
      <div class="glass"></div>
      <div class="cont">

        <div>
        <p>Leave information to<br>free consultation</p>
        </div>

        <div class="r-cont">
          <p class="title">Your information</p>
          <input type="text" placeholder="Your Name">
          <input type="text" placeholder="Email Address">
    <input type="text" placeholder="Phone Number"> 
    <p class="label">Tell us about your choice</p> 
   <input style="height:50px;" type="text" placeholder="">
    <input type="text" placeholder="Appropriate time frame (Optional)">
    <button>submit</button>

        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .container {
    position: relative;
  }
  
  .image-container img {
    width: 100%;
    height: 500px;
    display: block;
  }
  
  .glass {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 500px;
    background-color: rgba(0, 0, 0, 0.8);
  }
  
  .cont {
   
    width: 100%;
    height: 500px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: absolute;
    top: 0;
    left: 0;
    padding-left: 10%;
    padding-right: 4%;

    color: white;
    font-size: 25px;
    font-family: 'Unbounded';
    font-weight: 400;
  }
  
  .r-cont {

    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 20px;
   
  }
  
  input {
    margin: 10px;
    color: white;
    padding: 10px;
    width: 550px; 
    border: 1px solid white;
    background-color: rgba(81, 81, 81, 0.2);;
  }
  
  .label {
    font-size: 12px;
    font-family: 'Open Sans';
    padding-left: 10px;
  }

  button {
  height: 2.3rem;
  width: 13rem;
  color:black;
  background-color: rgb(255, 247, 0);
  font-size: 12px;
  font-family: 'Unbounded';
  font-weight: 700;
  border: 0px;
  margin-top: 4px;
  margin-left: 10px;
}
input::placeholder {
  color:rgb(207, 207, 207);
  font-size:12px;
}
  </style>
  