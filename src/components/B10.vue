<template>
  <div>
    <h1>bai 10</h1>
    <button @click="change1">an </button>
    <button @click="change2">hien</button>
    <p v-show="isVisible"> gia tri bi an</p>
    <p v-if="!isVisible">gia tri bi hien</p>
  </div>
</template>

<script setup>
import { ref } from "vue";
const isVisible = ref(false);

const change1 = () => {
  isVisible.value =true;
};

const change2 = () => {
  isVisible.value = false;
};
</script>

<style>

</style>