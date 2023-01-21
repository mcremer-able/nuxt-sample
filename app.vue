<template>
  <div>
    {{ data }}
  </div>
</template>
<script setup lang="ts">
const { data } = await useFetch<{ id: number }>(
  `https://jsonplaceholder.typicode.com/todos/1`
);
console.log(data.value);
</script>
