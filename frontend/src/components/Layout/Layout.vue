<script setup>
import  Navbar  from '../Navbar/Navbar.vue';
import  TabContent  from '../TabContent/TabContent.vue';

</script>

<template>
    <div class="layout">
        <div class="left">
            <Navbar/>
    </div>
    <div class="right">
        <TabContent/>
      
    </div>

    </div>
    
  </template>
  
  <style>
  

    .layout {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
    .left {
        width: 300px;
    }
    .right {
        width: 100%;
    }
    
  
  </style>
  