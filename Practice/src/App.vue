<script setup>

import { onMounted, ref } from "vue";

const count = ref(0);

const add = () => {
  count.value++;
}

const increment = () => {
  count.value = count.value + 2;
}

onMounted(()=> {
  console.log(count.value);
})

</script>

<template>
  <div>
    <h1>Vue: {{ count }}</h1>
    <button @click="add">加一</button>
    <button @click="increment">加二</button>
  </div>
</template>

<style></style>