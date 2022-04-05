<script setup>
defineEmits(['clickMe'])
const prop = defineProps({
  buttonName: {
    type: String,
    require: true,
    default: 'OK'
  }
})
console.log(prop.buttonName)
</script>

<template>
  <button @click="$emit('clickMe', $event, 100)">
      {{ buttonName }}
  </button>
</template>

<style></style>
