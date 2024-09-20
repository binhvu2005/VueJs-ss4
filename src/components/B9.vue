<template>
    <div>
        <h1>bai 9</h1>
      <h1>Danh sách bài viết</h1>
      <ul>
        <li v-for="product in products" :key="product.id">
          <h2>{{ product.title }}</h2>
          <p>{{ product.content }}</p>
          <small>Tác giả: {{ product.author }}</small>
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  const products = ref([
    {
      id: 1,
      title: 'Học Vue.js cơ bản',
      content: 'Vue.js là một framework mạnh mẽ để phát triển ứng dụng web.',
      author: 'Nguyễn Văn A'
    },
    {
      id: 2,
      title: 'Tìm hiểu về v-for trong Vue',
      content: 'v-for là một directive trong Vue.js cho phép lặp qua danh sách.',
      author: 'Trần Thị B'
    },
    {
      id: 3,
      title: 'Hướng dẫn sử dụng Vue Router',
      content: 'Vue Router giúp tạo ra các ứng dụng Vue.js có khả năng điều hướng.',
      author: 'Lê Văn C'
    }
  ]);
  </script>
  
  <style scoped>
  
  </style>
  