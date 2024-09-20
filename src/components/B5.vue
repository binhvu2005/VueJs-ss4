<template>
  <div>
    <h1>bai 5</h1>
    <h2>gio hang</h2>
    <span>con mua men men 1, so luong {{data.data1}}</span> <button @click="tangSoLuong1">tang so luong</button>
    <br>
    <span>con mua men women 1, so luong {{data.data2}}</span><button @click="tangSoLuong2">tang so luong</button>
    <br>
    <span>tong cong: {{data.data1 + data.data2}}</span>

  </div>
</template>

<script setup>
import { ref,reactive } from "vue";
const data = reactive({
    data1: 1,
    data2: 1
})

function tangSoLuong1() {
    data.data1++
   
}
function tangSoLuong2() {
    data.data2++
}

</script>

<style>

</style>