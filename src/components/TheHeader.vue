<template>
  <header>
    <h1>{{ props.title }}</h1>
    <p>{{ props.description }}</p>
    </header>
</template>

<script setup>
   import {defineProps} from 'vue';
   const props = defineProps({
     title:{
       type: String,
       default:'Welcome!'
     },
     description:{
       type: String,
       default: 'Have Fun This Summer!'
     }
   });
   </script>

   <style>
   h1 {
       width: 100%;
    color: rgb(116, 16, 16);
    text-align: center;
   }

   p {

    text-align: center;
    font-family: Georgia, "Times New Roman", Times, serif;
    font-size: 2rem;
    color: rgb(255, 0, 0);
 
   }
   </style>