<template>
  <p :id="route.params.id" v-if=true>Post {{ route.params.id }}</p>
  <p>Showing some raw html: <span v-html="rawHtml"></span></p>
</template>

<script setup>
const route = useRoute();

let rawHtml = '<span style="color:blue"> This should be blue </span>'
</script>