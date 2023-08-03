<template>
    <div class="bg">
      <div class="outline">
        <div class="row">
          <div class="first">
            <widget
              title="Phone Number"
              phoneNumber="+918220761220"
              imageSrc="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/ll.png?alt=media&token=8a6aad6c-f255-4ebe-874c-c232e86c25c2"
            />
            <widget
              title="Email"
              phoneNumber="samchris@gmail.com"
              imageSrc="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/opp.png?alt=media&token=250e639e-e484-46bc-af5b-bee30214460a"
            />
          </div>
          <textfield buttonText="Submit" initialValue="" />
        </div>
        <div class="horizontal-line"></div>
  
        <div class="components">
          <div class="card1">
            <div class="con">
              <p class="header">Best Woods</p>
              <p class="para">Best Woods Furniture Specializes in crafting high-quality, custom furniture for a variety of clients including individuals, interior designers, and commercial properties.</p>
            </div>
            <card3 :itemList="company" header="Company" />
            <card3 :itemList="Rooms" header="Rooms" />
            <card3 :itemList="links" header="Important Link" />
          </div>
        </div>
        <div class="horizontal-line"></div>
  
        <div class="foot-con">
          <div class="div1">
            <p class="cpy">Copyright © 2023 Best Woods. All rights reserved.</p>
          </div>
          <div class="div2">
            <p class="cpy">Back to Top ↑</p>
          </div>
          <div class="div3">
            <p class="cpy">Follow us</p>
            <img src="https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/soc.png?alt=media&token=96de8762-7d6d-4e0b-bbb8-6e76b97f0d6b" />
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import card3 from './card3.vue';
  import widget from './footer_layout.vue';
  import textfield from './textfield_footer.vue';
  
  export default {
    name: 'footer',
    components: {
      card3,
      widget,
      textfield,
    },
    data() {
      return {
        company: [
          { id: 1, text: '-- About us' },
          { id: 2, text: '-- Inspiration for you' },
          { id: 3, text: '-- Blogs' },
          { id: 4, text: '-- Contact us' },
        ],
        Rooms: [
          { id: 1, text: '-- Bed Room' },
          { id: 2, text: '-- Living Room' },
          { id: 3, text: '-- Study Room' },
          { id: 4, text: '-- Dining Room' },
          { id: 4, text: '-- Store Room' },
        ],
        links: [
          { id: 1, text: '-- FAQ' },
          { id: 2, text: '-- Terms & Condition' },
          { id: 3, text: '-- Privacy' },
          { id: 4, text: '-- Cookies Policy' },
          { id: 4, text: '-- Copyright Information' },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .bg {
    height: 520px;
    background-color: black;
    width: 100%;
    align-items: center;
    justify-content: start;
    display: flex;
    flex-direction: column;
  }
  
  .outline {
    padding-top: 30px;
    margin-top: 40px;
    margin-bottom: 40px;
    height: 90%;
    border: 1px solid white;
    display: flex;
    flex-direction: column;
    width: 95%;
  }
  
  .first {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
  }
  
  .row {
    padding-left: 20px;
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
  }
  
  .horizontal-line {
    display: inline;
    padding-top: 30px;
    width: 100%;
    margin-bottom: 10px;
    border-bottom: 1px solid grey;
  }
  
  .header {
    font-family: 'Unbounded';
    font-size: 18px;
    font-weight: 500;
    color: white;
  }
  
  .components {
    padding-top: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: start;
    align-items: center;
  }
  
  .card1 {
    display: flex;
    align-items: flex-start;
    justify-content: center;
  }
  
  .para {
    padding-top: 13px;
    font-family: 'Open Sans';
    font-size: 12px;
    font-weight: 500;
    color: grey;
  }
  
  .con {
    display: inline;
    width: 27%;
    margin-left: 20px;
    margin-right: 10%;
  }
  
  .cpy {
    font-family: 'Open Sans';
    color: white;
    font-size: 12px;
  }
  
  .foot-con {
    margin: 8px 20px;
    width: 95%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .div3 {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  img {
    width: 130px;
    padding-left: 20px;
  }
  </style>
  