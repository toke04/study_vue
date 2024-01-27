<script setup>
import {reactive} from "vue";

const user = reactive({name: "takashi"})

const alertName = () => {
  alert(`${user.name}です！`)
}

</script>

<template>
<div>
    <input v-model="user.name">
    <p> {{ user.name }}</p>
    <button @click="alertName">alert!</button>
</div>
</template>
