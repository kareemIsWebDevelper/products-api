<template>
<div>
    Counter: {{ counter }}
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
</div>
</template>
  
<script setup>
// state management
const counter = useCounter()
const increment = () =>{
    counter.value +=1 
} 
const decrement = () =>{
    counter.value -=1 
} 
</script>
  