<template>
    <div class="bg">
      <div class="container">
        <div class="header">
          <p class="title">Inspired by Room</p>
          <p class="contents">Whether you're looking to make a few simple updates or undertake a major home renovation, our journal is an invaluable resource that can help bring your home design vision to life. So why wait? Start exploring today and discover all the ways you can make your home the place you've always dreamed of.</p>
        </div>
        <div class="horizontal-line"></div>
        <Button :buttons="buttons"/>
        <div class="image">
          <img src="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/WhatsApp%20Image%202023-08-02%20at%208.11.20%20PM.jpeg?alt=media&token=0f5be46c-367d-4359-871f-524b29eb2f0e" alt="">
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import Button from './buttons.vue';
  
  export default {
    components: {
      Button,
    },
    data() {
      return {
        buttons: [
          {
            text: 'Bedroom',
            customClass: 'btn-primary', 
          },
          {
            text: 'Living Room',
            customClass: 'btn-secondary', 
          },
          {
            text: 'Dining Room',
            customClass: 'btn-primary', 
          },
          {
            text: 'Store Room',
            customClass: 'btn-primary', 
          },
          {
            text: 'Study Room',
            customClass: 'btn-primary', 
          },
          {
            text: 'Home Office',
            customClass: 'btn-primary', 
          },
        ],
      };
    },
    methods: {
      handleButtonClick(index) {
        console.log('Button clicked:', this.buttons[index].text);
      },
    },
  };
  </script>

  

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Open+Sans");
@import url("https://fonts.googleapis.com/css?family=Unbounded");



  .container .header .title {
    width: 700px;
    font-size: 22px;
    font-family: 'Unbounded';
    margin-bottom: 20px;
  }


  .container .header .contents {
    font-size: 13px;
    font-family: 'Open Sans';
    color:black;
    font-weight: 500;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);

  }


  .container {
    max-width: 100%;
    height: 655px;
    padding: 20px;
    border: 1px solid #000000;
    background-color: transparent;

  }

  .header {
    display: flex;
    align-items: start;
    justify-content: space-between;
    background-color: transparent;

  }
  
  .bg{
    max-width: 100%;
    height: 730px;
    padding:40px;
    background: linear-gradient(to bottom,rgb(245,245,245,245),rgb(255,240,247,255));
   
  }
  
  img{
    width:100%;
    height:475px

  }

  .horizontal-line {
    padding: 10px;
    margin-bottom: 10px;
  border-bottom: 1px solid grey;
}


</style>