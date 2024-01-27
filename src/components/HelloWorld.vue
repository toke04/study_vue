<script setup lang="ts">
import { ref } from 'vue'
defineProps<{ msg: string }>()
const count = ref(0)

const increCount = () => {
  if (count.value < 7){
    count.value++;
  } else{
    count.value = 0;
  }
}

</script>

<template>
  <h1>{{ msg }}</h1>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
