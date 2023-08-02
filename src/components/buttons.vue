<template>
    <div>
      <button
        v-for="(button, index) in buttons"
        :key="index"
        @click="handleClick(index)"
        :class="{ active: button.active, button: true }"
      >
        {{ button.text }}
      </button>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      buttons: {
        type: Array,
        required: true,
      },
    },
    methods: {
      handleClick(index) {
        if (index >= 0 && index < this.buttons.length) {
          const button = this.buttons[index];
          // Toggle the active state of the button
          button.active = !button.active;
        }
      },
    },
  };
  </script>
  
  <style scoped>
  @import url("https://fonts.googleapis.com/css?family=Unbounded");
  
  button {
    background-color: transparent;
    font-family: 'Unbounded';
    display: inline;
    align-self: self-end;
    justify-self: self-end;
    border: 1px solid grey;
    margin-top: 10px;
    margin-right: 5px;
    margin-bottom: 12px;
    padding-left: 44px;
    padding-top: 7px;
    padding-bottom: 7px;
    padding-right: 44px;
  }
  
  button.active {
    background-color: yellow;
    border-bottom: 3px  solid black;
    border-right: 3px  solid black;
   
  }
  </style>
  