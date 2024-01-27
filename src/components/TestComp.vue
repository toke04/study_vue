<template>
    <p>{{ count }}</p>
    <button @click="count++">ボタンです！</button>
</template>

<script setup>
import {ref} from "vue";
const count = ref(0)
</script>




