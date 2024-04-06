<template>
  <div :class="border">
    <p :id="route.params.id" v-if="false === false">Post {{ route.params.id }}</p>
    <p>Showing some raw html: <span v-html="rawHtml"></span></p>
  </div>

</template>

<script setup>
const route = useRoute();

let rawHtml = '<span style="color:blue"> This should be blue </span>'

const truthyValue = () => {
  return false
}
</script>

<style scoped>
div {
  border: 1px solid black;
  padding: 5px;
}
</style>
