<template >
    <v-app-bar class="fadeIn" color=#020201 flat>
    
      <v-app-bar-title class="custom-font ">
  
        <div class="wrapper">
          <!-- <v-icon icon="mdi-bullseye" /> -->
          ‎   TAURIFORM ‎  
        </div>
  
      </v-app-bar-title>
    </v-app-bar>
  
  </template>
  
  <script lang="ts" setup>
    //
  
  
  </script>
  
  
  <style scoped>
    @import '../fonts/custom-font.css';
  
    .custom-font {
    font-family: 'CustomFont', sans-serif;
    font-size: 1.2em;
    letter-spacing: 0.1em;
  
    /* Add other styling as needed */
  }
  
  .wrapper {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: center;
    gap: 0.5em;
  }

  .fadeIn {
  opacity: 0;
  animation: fadeIn 3s forwards;
  animation-delay: 1s;
}


@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
  
  
  
  </style>