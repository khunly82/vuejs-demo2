<script setup lang="ts">
import { ref, watchEffect } from 'vue';
import Alert from './components/Alert.vue';
const visible = ref<boolean>(false);
watchEffect(() => {
    console.log(visible.value)
})
</script>

<template>
    <button @click="visible = true">click me !!</button>
    <Alert message="Attention !!" v-model:visible="visible"></Alert>
</template>
<style scoped>
</style>
