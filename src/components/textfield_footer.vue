<!-- ButtonWithTextField.vue -->
<template>
    <div class="button-with-textfield">
        <input
        v-model="textFieldValue"
        @input="handleInput"
        class="custom-textfield"
        placeholder="Enter Email Address"
      />
      <button @click="handleClick" class="custom-button">{{ buttonText }}</button>
      
    </div>
  </template>
  
  <script>
  export default {
    props: {
      buttonText: String,
      initialValue: String
    },
    data() {
      return {
        textFieldValue: this.initialValue || ''
      };
    },
    methods: {
      handleClick() {
        this.$emit('click', this.textFieldValue);
      },
      handleInput() {
        this.$emit('input', this.textFieldValue);
      }
    }
  }
  </script>
  
  <style>

  @media (min-width: 901px) {
    
  
    .button-with-textfield {
      margin-left: 60px;
    margin-right:10px ;
    padding-left:10px;
    display:inline-block;
    text-align: center  ;
    justify-content: flex-end;
    border: 1px solid #ccc;
   
  }
  
  .custom-button {
    background-color:rgb(255, 247, 0);
    color: black;
    border: none;
    cursor: pointer;
    font-family: 'Unbounded';
    font-size: 12px;
    width: 120px;
    padding:5px;
    margin-right: 5px;
    margin-bottom: 3px;


  }
  
  .custom-textfield {
    background-color: transparent;
    margin-top: 10px;
    border:0px;
    font-size: 12px;
    width: 200px;
    caret-color: white;
    font-family: 'Unbounded';
    color:white
  }

  input:focus{
    outline: none;
  }
}

@media (max-width:900px) {
  .button-with-textfield {
    margin-top:12px;
    padding-left:10px;
    display: inline-block;
    justify-content: center;
    align-items: center;
    border: 1px solid #ccc;
   
  }
  
  .custom-button {
    background-color:rgb(255, 247, 0);
    color: black;
    border: none;
    cursor: pointer;
    font-family: 'Unbounded';
    font-size: 5px;
    padding:5px 20px;
    margin-right: 5px;
    margin-bottom: 5px;


  }
  
  .custom-textfield {
    background-color: transparent;
    margin-top: 10px;
    border:0px;
    font-size: 7px;
    width: 190px;
    caret-color: white;
    font-family: 'Unbounded';
    color:white
  }

  input:focus{
    outline: none;
  }
}
  </style>
  