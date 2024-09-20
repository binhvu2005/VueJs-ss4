<template>
    <div>
      <h1>bai 7</h1>
      <input type="number" v-model.number="myValue" placeholder="Nhập giá sản phẩm"/> 
      <button @click="addToCart">Add to cart</button>
      <p>gia tri hien tai: {{ price}}</p>
      <p>gia tri binhn phuong {{powerPrice}}</p>
    </div>
  </template>
  
  <script setup>
  import { ref, computed, watch } from 'vue';
  const myValue = ref (0)
  const price = ref(0);

  watch(price, (newVal, oldVal) => {
    console.log(`data changed from ${oldVal} to ${newVal}`);
  })


  const addToCart = () => {
    price.value = myValue.value 
    myValue.value = 0; 
  };
  
  const powerPrice = computed(() => {
    return price.value*price.value 
  });
  </script>
  
  <style>
  </style>
  