<template>
  <div>
    <h1>bai 2</h1>
    <p>company : {{user.company}}</p>
    <p>age : {{user.age}}</p>
    <button @click="changeData">change data</button>
  </div>
</template>

<script setup>
import { reactive } from "vue";
const user = reactive ({
    company : "rikkei academy",
    age : 1
})

function changeData() {
    user.company =  "rikkei education"
    user.age = 2
}
</script>

<style>

</style>