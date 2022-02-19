<script setup>
import { ref } from 'vue'
const textKey = ref([])
document.body.addEventListener('keydown', (e) => {
  textKey.value.push(e.which)
});

</script>
 
<template>
  <div style="margin: 2em;">
    <h1>{{ textKey }}</h1>
  </div>
</template>

<style>

</style>