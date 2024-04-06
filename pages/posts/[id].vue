<template>
  <p>Post</p>
</template>
<script setup>
const route = useRoute();

console.log("Route parameter:", route.params.id)
</script>