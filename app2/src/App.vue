<script setup>
import BaseButtonVue from './components/BaseButton.vue';
const testMe1 = () => console.log('test me 1')
const testMe2 = (e) => console.log('test me 2', e)
const testMe3 = (e) => console.log('test me 3', e)
const testMe4 = (e, n) => console.log('test me 4', e, n)
const testMe5 = (e, n) => console.log('test me 5', e, n)
const testMe6 = (e, n) => console.log('test me 6', e, n)
</script>

<template>
  <div>
    <div>
      <button @click="testMe1">TEST ME 1</button>
      <button @click="testMe2">TEST ME 2</button>

      <button @click="testMe3()">TEST ME 3</button>
      <button @click="testMe4($event)">TEST ME 4</button>

      <button @click="testMe5($event, 999)">TEST ME 5</button>
      <button @click="testMe6(999, $event)">TEST ME 6</button>
    </div>
    <BaseButtonVue></BaseButtonVue>
  </div>
</template>

<style></style>
